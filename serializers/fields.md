name, description, type
ago, How long ago this was created , string
alt_email, The alt email address of this user; should only show if this is active user profile, string
app_language, Info on the language setting chosen by this user, object; AppLanguage
attended_events, The events (visible to the active user) that this user has attended, array; AttendedEvent
bio, Description of this user, string
body, Content of the post, string
can_edit_profile, "Whether the active user can edit this profile", boolean
can_message, Whether the active user can message this user, boolean
connection_status, Info on connection status between this and active user, object; UserConnectionShort
description, The description of this group, string
email, The email address of this user; should only show if this is active user profile, string
event, Info on the event, object; EventTiny
event_council_member, Whether this user is an event_council_member for this event,boolean
event_notes, Any event notes that the active user may have created for this user , array; EventNoteShort
first_name, "The user's first name", string
group_id, The ID of the group, integer
group_invite_id, The ID the group invite, integer
group_request_id, The ID of the group request, integer
group_type, Info about the type of this group ,object; GroupTypeShort
group_type_name, The name of the group_type of this group, string
groups, The groups (visible to the active user) that this user belongs to, array; GroupTiny
id, The ID of this record, integer
is_approval_required, Whether the user needs to be approved to join, boolean
is_content_visible, Whether posts are visibile, boolean
is_group_visible, Whether the group can be seen, boolean
is_memberlist_visible, Whether the member list can be seen, boolean
is_viewed, Whether the active user has previously viewed this, boolean
last_name, "The user's last name", string
name, The name of this group, string
organization_name, "The organization the user is associated with", string
owner, Info about the group owner, object; UserShort
owner_user_id, The user ID of the user who owns this group, integer
photo, URL of a photo of the user, string
post_count, How many posts (visible to the active user) this user has created, integer
post_id, The ID of the post, integer
post_like_count, How many post likes (visible to the active user) this user has created, integer
title, "The user's title", string
user, Info on the user, object; UserTiny
user_connection, Info on the connection between active user and other user, object; UserConnectionShort
user_connection_count, How many connections (visible to the active user) this user has created, integer
user_connections_blocked, Whether the active user can connect with this user, boolean
user_profile, "Whether the user has a profile, usually used for speakers who don't have full profiles", boolean
user_role_id, "The ID of this user's role", integer