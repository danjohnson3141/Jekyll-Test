name, description, type
address, The steet address for this event, string
ago, How long ago this was created, string
allow_bookmarks, Whether the active user can bookmark things, boolean
allow_notes, Whether the active user can create event_notes, boolean
alt_email, The alt email address of this user; should only show if this is active user profile, string
app_language, Info on the language setting chosen by this user, object; AppLanguage
attended_events, The events (visible to the active user) that this user has attended, array; AttendedEvent
begin_date, The day that the event begins; yyyy-mm-dd, string
bio, Description of this user, string
body, Content of the post, string
can_edit_profile, "Whether the active user can edit this profile", boolean
can_follow_event, Whether the active user can follow this event, boolean
can_message, Whether the active user can message this user, boolean
city, The city in which the event is happening, string
connection_status, Info on connection status between this and active user, object; UserConnectionShort
country, Info on the country this event is happening in, object; Country
description, The description of this group, string
description, Verbose name of locale; used externally, string
email, The email address of this user; should only show if this is active user profile, string
end_date, The day that the event ends; yyyy-mm-dd, string
event, Info on the event, object; Event
event, Info on the event, object; EventShort
event, Info on the event, object; EventTiny
event_council_member, Whether this user is an event_council_member for this event,boolean
event_evaluations, All of the event evaluations visible to the active user for this event, array; EventEvaluation
event_follower_id, If the active user is following the event; this is the ID of that record, integer
event_id, The ID of the event, integer 
event_notes, Any event notes that the active user may have created for this user, array; EventNoteShort
event_notes, Any event notes that the active user may have created for this user, array; EventNoteTiny
event_registration_status, Info on this users reg status, object; EventRegistrationStatus
event_session, Info on the event_session, object; EventSession
event_session, Info on the event_session, object; EventSessionShort
event_session_id, The ID of the event_session, integer 
event_speaker, Info on the event_speaker, object; EventSpeaker
event_speaker, Info on the event_speaker, object; EventSpeakerShort
event_speaker_id, The ID of the event_speaker, integer 
event_staff, List of event staff, array; UserShort
event_user, Info on the event_user, object; EventUser
event_user, Info on the event_user, object; EventUserTiny
event_user_id, The ID of the event_user, integer 
first_name, "The user's first name", string
group, Info on the group this event is associated with, object; GroupTiny
group_id, The ID of the group, integer
group_invite_id, The ID the group invite, integer
group_request_id, The ID of the group request, integer
group_type, Info about the type of this group,object; GroupTypeShort
group_type_name, The name of the group_type of this group, string
groups, The groups (visible to the active user) that this user belongs to, array; GroupTiny
id, The ID of this record, integer
is_approval_required, Whether the user needs to be approved to join, boolean
is_approved, Whether this connection request has been approved, boolean
is_approver, Whether the active user is the person to approve this request, boolean
is_content_visible, Whether posts are visibile, boolean
is_group_visible, Whether the group can be seen, boolean
is_memberlist_visible, Whether the member list can be seen, boolean
is_viewed, Whether the active user has previously viewed this, boolean
key, The reference used by the app to associate this text with the on page element, string
label, The actual text displayed by the app, string
label_plural, Plural of the label; if neccesary, string
last_name, "The user's last name", string
name, The name of this event, string
name, The name of this group, string
name, The name of this region, string
name, The named used internally; usually two characters, string
organization_name, "The organization the user is associated with", string
owner, Info about the group owner, object; UserShort
owner_user_id, The user ID of the user who owns this group, integer
photo, URL of a photo of the user, string
post_count, How many posts (visible to the active user) this user has created, integer
post_id, The ID of the post, integer
post_like_count, How many post likes (visible to the active user) this user has created, integer
postal_code, Postal code for the event, string
registraion_status, The registration status of the active user for this event, string
sponsor, Info on the sponsor, object; Sponsor
sponsor, Info on the sponsor, object; SponsorTiny
sponsor_id, The ID of the sponsor, integer 
sponsors, List of sponsors, array; SponsorShort
state, The state in which the event is happening, string
timezone, Info on the timezone this event is happening in, object: Timezone
title, "The user's title", string
user, Info on the user, object; User
user, Info on the user, object; UserMicro
user, Info on the user, object; UserNano
user, Info on the user, object; UserShort
user, Info on the user, object; UserTiny
user_connection, Info on the connection between active user and other user, object; UserConnectionShort
user_connection_count, How many connections (visible to the active user) this user has created, integer
user_connections_blocked, Whether the active user can connect with this user, boolean
user_profile, "Whether the user has a profile, usually used for speakers who don't have full profiles", boolean
user_role_id, "The ID of this user's role", integer
user_today_event, Whether the event is happening today, boolean
venue_name, The name of the location where the event is happening, string
client_id, A reference key to an external record, string
display_rank, Allows for arbitrary sorting of results, integer
event_council, Info on the event_council, object; EventCouncil
leaderboard_points, The cumulative number of points this user has, integer