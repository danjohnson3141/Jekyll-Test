[[Gollum]]

Changes made to the files locally in a text editor will not be reflected on the wiki till they're committed to the repository.

Evanta Access is a social networking and event management Application that is currently being used as  collaborative tool amongst the CXOs of many Fortune 1000 companies. These APIs allow the user to interact with the network.

The types of API routes available can generally be broken up into seven different categories:

* [[App-&-Navigation]]
* [[Events]]
* [[Groups]]
* [[Messages]]
* [[Posts]]
* [[Users]]
* [[All Routes]]


***


===
####Pagination

If the API request is designed to return more than one record, it is possible to paginate the results by adding the following suffix to the end of the request `?page=#&per_page=#`.

So the message route of `GET /messages` would become `GET /messages?page=2&per_page=3`

___

####Templates
This is the template currently being used for new documentation: [[Template]]

Possibly using this as a template: http://wiki.alfresco.com/wiki/API_Reference_Template

Would eventually like to look like Twitter's: https://dev.twitter.com/docs/api/1.1

[[These are routes that still need documenation|Routes-that-need-documentation]]

Helpful API documentation resources:

* http://www.monperrus.net/martin/how-to-write-good-API-documentation