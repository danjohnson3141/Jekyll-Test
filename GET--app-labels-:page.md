GET /app/labels/:page

There are no form parameters for this route. All parameters are passed in through the URL by asking for the page name.

JSON response example:

```
{"app_label_pages"=>
  [{"id"=>10,
    "key"=>"Test Dictionary",
    "label"=>"Testing Label Text",
    "label_plural"=>nil}]}

```