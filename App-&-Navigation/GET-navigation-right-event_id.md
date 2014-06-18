<!-- --- title: GET /navigation/right/:event_id -->

This returns the elements for the right navigation bar. Each of the buttons can be turned on and off by various app_setting records. 

=
####Authentication:

The user needs to be logged in and have valid credentials to use this route.

=
####Parameters:

:event_id - Integer, passed in through the URL. Derived from the 'id' field of the 'events' table.

=
####API request example:
```html
http://example.com/navigation/right/234
```

=
####JSON response example:

```json
{
    "navigation_right": {
        "show_attendees": true,
        "show_sessions": true,
        "show_my_schedule": true,
        "show_sponsors": true,
        "show_speakers": true,
        "show_qr_scannable": true,
        "show_qr_scanner": true,
        "show_event_notes": true,
        "show_bookmarks": true,
        "show_leaderboard": true,
        "show_leaderboard_rules": true,
        "show_event_evaluations": true
    }
}
```

This requests provides a <strong>HTML 200</strong> on success.