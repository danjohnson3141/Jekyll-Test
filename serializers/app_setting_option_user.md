| name           | description                                                                               | type    |
|----------------|-------------------------------------------------------------------------------------------|---------|
| id             | The ID of this record                                                                     | integer |
| app_setting_id | If this setting is enabled references the record of it so that it can be modified/deleted | integer |
| category       | A broad classification of this app setting                                                | string  |
| description    | A narrower classification of this app setting                                             | string  |
| name           | The name of the setting from the database                                                 | string  |
| setting        | Whether this setting is enabled or not                                                    | boolean |
| app_label      | The text to be displayed in the app from the labels table                                 | string  |