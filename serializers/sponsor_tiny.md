| name           | description                                       | type  attributes     |
|----------------|---------------------------------------------------|----------------------|
| id             | The ID of this record                             | integer              |
| name           | The name of this sponsor                          | string               |
| description    | The description of this sponsor                   | string               |
| logo           | URL of the image associated with this sponsor     | string               |
| url            | URL of the desired external link for this sponsor | string               |
| splash_sponsor | Whether this sponsor is a splash sponsor          | boolean              |
| sponsor_type   | Info on the type of sponsor                       | object; SponsorType  |
| banner_ads     | Any banner ads associated with this sponsor       | array; BannerAdShort |