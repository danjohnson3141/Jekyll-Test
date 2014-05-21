name, description, type
id, The ID of this record, integer
name, , string
begin_date, The day that the event begins; yyyy-mm-dd, string
end_date, The day that the event ends; yyyy-mm-dd, string
venue_name, The name of the location where the event is happening, string
address, The steet address for this event, string
city, The city in which the event is happening, string
state, , string
postal_code, , string
event_follower_id, , integer
registraion_status, , string
user_today_event, Whether the event is happening today , boolean
can_follow_event, Whether the active user can follow this event, boolean
allow_notes, Whether the active user can create event_notes, boolean
allow_bookmarks, Whether the active user can bookmark things, boolean
country, Info on the country this event is happening in, object; country
timezone, Info on the timezone this event is happening in, object: timezone
group, Info on the group this event is associated with, object; GroupTiny
sponsors, List of sponsors, array; SponsorShort
event_staff, List of event staff , array; UserShort
event_evaluations, All of the event evaluations visible to the active user for this event, array; EventEvaluation