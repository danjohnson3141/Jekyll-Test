name, description, type
id, The ID of this record, integer
name, ,
begin_date, ,
end_date, ,
venue_name, ,
address, ,
city, ,
state, ,
postal_code, ,
event_follower_id, ,
registraion_status, ,
user_today_event, ,
can_follow_event, ,
allow_notes, ,
allow_bookmarks, ,
country, , object; country
timezone, , object: timezone
group, , object; GroupTiny
sponsors, , array; SponsorShort
event_staff, , array; UserShort
event_evaluations, , array; event evaluations

  def event_evaluations
    object.get_event_evaluations(scope)
  end

  def event_follower_id
    EventFollower.where(user_id: current_user.id, event_id: self.id).first.try(:id)
  end

  def registraion_status
    event_user = EventUser.where(user_id: current_user.id, event_id: self.id).first
    registration_status = EventRegistrationStatus.find(event_user.event_registration_status_id).key if event_user && !event_user.event_registration_status_id.nil?
  end

  def user_today_event
    return false if AppSettings::Value.new(:todays_event_callout, event: object).off?
    object.user_today_event?(scope)
  end

  def can_follow_event
    object.can_follow_event?
  end

  def attendees
    return object.attendees_excluding_hidden if object.show_attendees?(current_user)
    []
  end

  def event_sponsors
    object.event_sponsors if object.show_event_sponsors?(scope)
  end

  def allow_notes
    AppSettings::Value.new(:event_notes, event: object, user: scope).on?
  end

  def allow_bookmarks
    AppSettings::Value.new(:event_bookmarks, event: object, user: scope).on?
  end



end
