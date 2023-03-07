# <p align="center" width="100%"> <img src="./logo.png" width="250" height="250"> </p>
# <p align="center" width="100%"> Intercom API OIH Connector </p>

## Description

A generated OIH connector for the Intercom API API (version 2.8).

Generated from: https://raw.githubusercontent.com/intercom/Intercom-OpenAPI/main/descriptions/2.8/api.intercom.io.yaml <br/>
Generated at: 2023-03-07T13:49:45+01:00 <br/>
Snapshot key: 

## API Description

The intercom API reference.<br/>

## Authorization

Supported authorization schemes:
- Bearer Token

## Actions

### Identify an admin
> You can view the currently authorised admin along with the embedded app object (a "workspace" in legacy terminology).<br/>
> <br/>
> >  Single Sign On<br/>
> ><br/>
> > If you are building a custom "Log in with Intercom" flow for your site, and you call the `/me` endpoint to identify the logged-in user, you should not accept any sign-ins from users with unverified email addresses as it poses a potential impersonation security risk.<br/>

*Tags:* `Admins`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List all admins
> You can fetch a list of admins for a given workspace.<br/>

*Tags:* `Admins`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve an admin
> You can retrieve the details of a single admin.<br/>

*Tags:* `Admins`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given admin<br/>

### List all articles
> You can fetch a list of all articles by making a GET request to `https://api.intercom.io/articles`.<br/>
> <br/>
> >  How are the articles sorted and ordered?<br/>
> ><br/>
> > Articles will be returned in descending order on the `updated_at` attribute. This means if you need to iterate through results then we'll show the most recently updated articles first.<br/>

*Tags:* `Articles`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Set an admin to away
> You can set an Admin as away for the Inbox.<br/>

*Tags:* `Admins`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given admin<br/>

### List all collections
> You can fetch a list of all collections by making a GET request to `https://api.intercom.io/help_center/collections`.<br/>
> <br/>
> >  How are the collections sorted and ordered?<br/>
> ><br/>
> > Collections will be returned in descending order on the `updated_at` attribute. This means if you need to iterate through results then we'll show the most recently updated collections first.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List all activity logs
> You can get a log of activities by all admins in an app.<br/>

*Tags:* `Admins`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `created_at_after` - _required_ - The start date that you request data for. It must be formatted as a UNIX timestamp.<br/>
* `created_at_before` - _optional_ - The end date that you request data for. It must be formatted as a UNIX timestamp.<br/>

### Delete a collection
> You can delete a single collection by making a DELETE request to `https://api.intercom.io/collections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the collection which is given by Intercom.<br/>

### Delete an article
> You can delete a single article by making a DELETE request to `https://api.intercom.io/articles/<id>`.<br/>

*Tags:* `Articles`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the article which is given by Intercom.<br/>

### Update an article
> You can update the details of a single article by making a PUT request to `https://api.intercom.io/articles/<id>`.<br/>

*Tags:* `Articles`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the article which is given by Intercom.<br/>

### Create a collection
> You can create a new collection by making a POST request to `https://api.intercom.io/help_center/collections.`<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve an article
> You can fetch the details of a single article by making a GET request to `https://api.intercom.io/articles/<id>`.<br/>

*Tags:* `Articles`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the article which is given by Intercom.<br/>

### Update a collection
> You can update the details of a single collection by making a PUT request to `https://api.intercom.io/collections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the collection which is given by Intercom.<br/>

### Retrieve a collection
> You can fetch the details of a single collection by making a GET request to `https://api.intercom.io/help_center/collections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the collection which is given by Intercom.<br/>

### List all sections
> You can fetch a list of all sections by making a GET request to `https://api.intercom.io/help_center/sections`.<br/>
> >  How are the sections sorted and ordered?<br/>
> ><br/>
> > Sections will be returned in descending order on the `updated_at` attribute. This means if you need to iterate through results then we'll show the most recently updated sections first.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Delete a section
> You can delete a single section by making a DELETE request to `https://api.intercom.io/sections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the section which is given by Intercom.<br/>

### Create an article
> You can create a new article by making a POST request to `https://api.intercom.io/articles`.<br/>

*Tags:* `Articles`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Update a section
> You can update the details of a single section by making a PUT request to `https://api.intercom.io/sections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the section which is given by Intercom.<br/>

### Create or Update a company
> You can create or update a company.<br/>
> <br/>
> >  Companies with no users<br/>
> ><br/>
> > Companies will be only visible in Intercom when there is at least one associated user.<br/>
> <br/>
> Companies are looked up via `company_id` in a `POST` request, if not found via `company_id`, the new company will be created, if found, that company will be updated.<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Delete a company
> You can delete a single company.<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### Retrieve a section
> You can fetch the details of a single section by making a GET request to `https://api.intercom.io/help_center/sections/<id>`.<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the section which is given by Intercom.<br/>

### Create a section
> You can create a new section by making a POST request to `https://api.intercom.io/help_center/sections.`<br/>

*Tags:* `Help Center`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a company
> You can fetch a company by either passing in `company_id` or `name` as a query parameter.<br/>
> <br/>
> A company can also be fetched by its name using a name or company_id parameter in the url, whose values are the ones you have defined for that company -<br/>
>   `https://api.intercom.io/companies?name={name}`<br/>
>   `https://api.intercom.io/companies?company_id={company_id}`<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `filter` - _required_

### Update a company
> You can update a single company<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### Retrieve a company by ID
> You can fetch a single company.<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### List attached segments for companies
> You can fetch a list of all segments that belong to a company.<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### Detach a contact from a company
> You can detach a company from a single contact.<br/>

*Tags:* `Companies` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### List all companies
> You can list companies. The company list is sorted by the `last_request_at` field and by default is ordered descending, most recently requested first.<br/>
> <br/>
> Note that the API does not include companies who have no associated users in list responses.<br/>
> <br/>
> > <br/>
> ><br/>
> > When using the Companies endpoint and the pages object to iterate through the returned companies, there is a limit of 10,000 Companies that can be returned. If you need to list or iterate on more than 10,000 Companies, please use the [Scroll API](https://developers.intercom.com/reference#iterating-over-all-companies).<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `page` - _optional_ - what page of results to fetch. Defaults to first page<br/>
* `per_page` - _optional_ - how many results per page. Defaults to 15<br/>
* `order` - _optional_ - `asc` or `desc`. Return the companies in ascending or descending order. Defaults to desc<br/>
* `filter` - _required_

### List attached contacts
> You can fetch a list of all contacts that belong to a company.<br/>

*Tags:* `Companies` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the company which is given by Intercom<br/>

### List attached companies for contact
> You can fetch a list of companies that are associated to a contact.<br/>

*Tags:* `Contacts` `Companies`

#### Input Parameters
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Scroll over all companies
> The `list all companies` functionality does not work well for huge datasets, and can result in errors and performance problems when paging deeply. The Scroll API provides an efficient mechanism for iterating over all companies in a dataset.<br/>
> <br/>
> - Each app can only have 1 scroll open at a time. You'll get an error message if you try to have more than one open per app.<br/>
> - If the scroll isn't used for 1 minute, it expires and calls with that scroll param will fail<br/>
> - If the end of the scroll is reached, "companies" will be empty and the scroll parameter will expire<br/>
> <br/>
> >  Scroll Parameter<br/>
> ><br/>
> > You can get the first page of companies by simply sending a GET request to the scroll endpoint. For subsequent requests you will need to use the scroll parameter from the response.<br/>
> <br/>
> >  Scroll network timeouts<br/>
> ><br/>
> > Since scroll is often used on large datasets network errors such as timeouts can be encountered. When this occurs you will need to restart your scroll query as it is not possible to continue from a specific point when using scroll.<br/>
> ><br/>
> > When this occurs you will see a HTTP 500 error with the following message:<br/>
> > "Request failed due to an internal network error. Please restart the scroll operation."<br/>

*Tags:* `Companies`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `scroll_param` - _optional_

### Attach a Contact to a Company
> You can attach a company to a single contact.<br/>

*Tags:* `Companies` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>

### Create a note
> You can add a note to a single contact.<br/>

*Tags:* `Notes` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given contact.<br/>

### List all notes
> You can fetch a list of notes that are associated to a contact.<br/>

*Tags:* `Notes` `Contacts`

#### Input Parameters
* `id` - _required_ - The unique identifier of a contact.<br/>
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Add subscription to a contact
> You can add a specific subscription to a contact. In Intercom, we have two different subscription types based on user consent - opt-out and opt-in:<br/>
> <br/>
>   1.Attaching a contact to an opt-out subscription type will opt that user out from receiving messages related to that subscription type.<br/>
> <br/>
>   2.Attaching a contact to an opt-in subscription type will opt that user in to receiving messages related to that subscription type.<br/>
> <br/>
> This will return a subscription type model for the subscription type that was added to the contact.<br/>

*Tags:* `Subscription Types` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>

### List attached segments for contact
> You can fetch a list of segments that are associated to a contact.<br/>

*Tags:* `Contacts` `Segments`

#### Input Parameters
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List tags attached to a contact
> You can fetch a list of all tags that are attached to a specific contact.<br/>

*Tags:* `Contacts` `Tags`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>

### Add tag to a contact
> You can tag a specific contact. This will return a tag object for the tag that was added to the contact.<br/>

*Tags:* `Tags` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>

### Remove tag from a contact
> You can remove tag from a specific contact. This will return a tag object for the tag that was removed from the contact.<br/>

*Tags:* `Tags` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `id` - _required_ - The unique identifier for the tag which is given by Intercom<br/>

### Remove subscription from a contact
> You can remove a specific subscription from a contact. This will return a subscription type model for the subscription type that was removed from the contact.<br/>

*Tags:* `Subscription Types` `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `id` - _required_ - The unique identifier for the subscription type which is given by Intercom<br/>

### List subscriptions for a contact
> You can fetch a list of subscription types that are attached to a contact. These can be subscriptions that a user has 'opted-in' to or has 'opted-out' from, depending on the subscription type.<br/>
> This will return a list of Subscription Type objects that the contact is associated with.<br/>
> <br/>
> The data property will show a combined list of:<br/>
> <br/>
>   1.Opt-out subscription types that the user has opted-out from.<br/>
>   2.Opt-in subscription types that the user has opted-in to receiving.<br/>

*Tags:* `Contacts` `Subscription Types`

#### Input Parameters
* `contact_id` - _required_ - The unique identifier for the contact which is given by Intercom<br/>
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Update a contact
> You can update an existing contact (ie. user or lead).<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - id<br/>

### Get a contact
> You can fetch the details of a single contact.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - id<br/>

### Delete a contact
> You can delete a single contact.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - id<br/>

### Create contact
> You can create a new contact (ie. user or lead).<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Merge a lead and a user
> You can merge a contact with a `role` of `lead` into a contact with a `role` of `user`.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Search contacts
> You can search for multiple contacts by the value of their attributes in order to fetch exactly who you want.<br/>
> <br/>
> To search for contacts, you need to send a POST request to `https://api.intercom.io/contacts/search`. This will accept a query object in the body which will define your filters in order to search for contacts.<br/>
> <br/>
> >  Why is there a delay when creating contacts and searching for them?<br/>
> ><br/>
> > If a contact has recently been created, there is a possibility that it will not yet be available when searching. This means that it may not appear in the response. This delay can take a few minutes. If you need to be instantly notified then you could use webhooks instead, which you'd currently have to iterate on to see if they match your search filters.<br/>
> <br/>
> >  Nesting & Limitations<br/>
> ><br/>
> > You can nest these filters in order to get even more granular insights that pinpoint exactly what you need. Example: (1 OR 2) AND (3 OR 4).<br/>
> > There are some limitations to the amount of multiple's there can be:<br/>
> > * There's a limit of max 2 nested filters<br/>
> > * There's a limit of max 15 filters for each AND or OR group<br/>
> <br/>
> >  Searching for Timestamp Fields<br/>
> <br/>
> > All timestamp fields (created_at, updated_at etc.) are indexed as Dates for Contact Search queries; Datetime queries are not currently supported. This means you can only query for timestamp fields by day - not hour, minute or second.<br/>
> > For example, if you search for all Contacts with a created_at value greater (>) than 1577869200 (the UNIX timestamp for January 1st, 2020 9:00 AM), that will be interpreted as 1577836800 (January 1st, 2020 12:00 AM). The search results will then include Contacts created from January 2nd, 2020 12:00 AM onwards.<br/>
> > If you'd like to get contacts created on January 1st, 2020 you should search with a created_at value equal (=) to 1577836800 (January 1st, 2020 12:00 AM).<br/>
> > This behaviour applies only to timestamps used in search queries. The search results will still contain the full UNIX timestamp and be sorted accordingly.<br/>
> <br/>
> ### Accepted Fields<br/>
> <br/>
> Most key listed as part of the Contacts Model are searchable, whether writeable or not. The value you search for has to match the accepted type, otherwise the query will fail (ie. as `created_at` accepts a date, the `value` cannot be a string such as `"foorbar"`).<br/>
> <br/>
> | Field                              | Type                           |<br/>
> | ---------------------------------- | ------------------------------ |<br/>
> | id                                 | String                         |<br/>
> | role                               | String<br>Accepts user or lead |<br/>
> | name                               | String                         |<br/>
> | avatar                             | String                         |<br/>
> | owner_id                           | Integer                        |<br/>
> | email                              | String                         |<br/>
> | phone                              | String                         |<br/>
> | external_id                        | String                         |<br/>
> | created_at                         | Date (UNIX Timestamp)          |<br/>
> | signed_up_at                       | Date (UNIX Timestamp)          |<br/>
> | updated_at                         | Date (UNIX Timestamp)          |<br/>
> | last_seen_at                       | Date (UNIX Timestamp)          |<br/>
> | last_contacted_at                  | Date (UNIX Timestamp)          |<br/>
> | last_replied_at                    | Date (UNIX Timestamp)          |<br/>
> | last_email_opened_at               | Date (UNIX Timestamp)          |<br/>
> | last_email_clicked_at              | Date (UNIX Timestamp)          |<br/>
> | language_override                  | String                         |<br/>
> | browser                            | String                         |<br/>
> | browser_language                   | String                         |<br/>
> | os                                 | String                         |<br/>
> | location.country                   | String                         |<br/>
> | location.region                    | String                         |<br/>
> | location.city                      | String                         |<br/>
> | unsubscribed_from_emails           | Boolean                        |<br/>
> | marked_email_as_spam               | Boolean                        |<br/>
> | has_hard_bounced                   | Boolean                        |<br/>
> | ios_last_seen_at                   | Date (UNIX Timestamp)          |<br/>
> | ios_app_version                    | String                         |<br/>
> | ios_device                         | String                         |<br/>
> | ios_app_device                     | String                         |<br/>
> | ios_os_version                     | String                         |<br/>
> | ios_app_name                       | String                         |<br/>
> | ios_sdk_version                    | String                         |<br/>
> | android_last_seen_at               | Date (UNIX Timestamp)          |<br/>
> | android_app_version                | String                         |<br/>
> | android_device                     | String                         |<br/>
> | android_app_name                   | String                         |<br/>
> | andoid_sdk_version                 | String                         |<br/>
> | segment_id                         | String                         |<br/>
> | tag_id                             | String                         |<br/>
> | custom_attributes.{attribute_name} | String                         |<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List all contacts
> You can fetch a list of all contacts.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Archive contact
> You can archive a single contact.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - id<br/>

### Unarchive contact
> You can unarchive a single contact.<br/>

*Tags:* `Contacts`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - id<br/>

### List all conversations
> You can fetch a list of all conversations.<br/>
> <br/>
> You can optionally request the result page size and the cursor to start after to fetch the result<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `per_page` - _optional_ - How many results per page<br/>
* `starting_after` - _optional_ - String used to get the next page of conversations.<br/>

### Remove tag from a conversation
> You can remove tag from a specific conversation. This will return a tag object for the tag that was removed from the conversation.<br/>

*Tags:* `Tags` `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `conversation_id` - _required_ - conversation_id<br/>
* `id` - _required_ - id<br/>

### Add tag to a conversation
> You can tag a specific conversation. This will return a tag object for the tag that was added to the conversation.<br/>

*Tags:* `Tags` `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `conversation_id` - _required_ - conversation_id<br/>

### Reply to a conversation
> You can reply to a conversation with a message from an admin or on behalf of a contact, or with a note for admins.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_

### Update a conversation
> You can update an existing conversation.<br/>
> <br/>
> > <br/>
> ><br/>
> > If you want to update a conversation with either a reply (or actions such as assign, unassign, open, close or snooze) then take a look at their own sections respectively as they currently require different endpoints and parameters.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The id of the conversation to target<br/>
* `display_as` - _optional_ - Set to plaintext to retrieve conversation messages in plain text.<br/>

### Creates a conversation
> You can create a conversation that has been initiated by a contact (ie. user or lead).<br/>
> The conversation can be an in-app message only.<br/>
> <br/>
> >  Sending for visitors<br/>
> ><br/>
> > You can also send a message from a visitor by specifying their `user_id` or `id` value in the `from` field, along with a `type` field value of `contact`.<br/>
> > This visitor will be automatically converted to a contact with a lead role once the conversation is created.<br/>
> <br/>
> This will return the Message model that has been created.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Search conversations
> You can search for multiple conversations by the value of their attributes in order to fetch exactly which ones you want.<br/>
> <br/>
> To search for conversations, you need to send a POST request to https://api.intercom.io/conversations/search. This will accept a query object in the body which will define your filters in order to search for conversations.<br/>
> <br/>
> >  Nesting & Limitations<br/>
> ><br/>
> > You can nest these filters in order to get even more granular insights that pinpoint exactly what you need. Example: (1 OR 2) AND (3 OR 4).<br/>
> > There are some limitations to the amount of multiple's there can be:<br/>
> > - There's a limit of max 2 nested filters<br/>
> > - There's a limit of max 15 filters for each AND or OR group<br/>
> <br/>
> ### Accepted Fields<br/>
> <br/>
> Most keys listed as part of the The conversation model is searchable, whether writeable or not. The value you search for has to match the accepted type, otherwise the query will fail (ie. as `created_at` accepts a date, the `value` cannot be a string such as `"foorbar"`).<br/>
> <br/>
> | Field                                     | Type                                                                                     |<br/>
> | :---------------------------------------- | :--------------------------------------------------------------------------------------- |<br/>
> | id                                        | String                                                                                   |<br/>
> | created_at                                | Date (UNIX timestamp)                                                                    |<br/>
> | updated_at                                | Date (UNIX timestamp)                                                                    |<br/>
> | source.type                               | String                                                                                   |<br/>
> | source.id                                 | String                                                                                   |<br/>
> | source.delivered_as                       | String                                                                                   |<br/>
> | source.subject                            | String                                                                                   |<br/>
> | source.body                               | String                                                                                   |<br/>
> | source.author.id                          | String                                                                                   |<br/>
> | source.author.type                        | String                                                                                   |<br/>
> | source.author.name                        | String                                                                                   |<br/>
> | source.author.email                       | String                                                                                   |<br/>
> | source.url                                | String                                                                                   |<br/>
> | contact_ids                               | String                                                                                   |<br/>
> | teammate_ids                              | String                                                                                   |<br/>
> | admin_assignee_id                         | String                                                                                   |<br/>
> | team_assignee_id                          | String                                                                                   |<br/>
> | channel_initiated                         | String<br>Accepted fields are `conversation`, `push`, `facebook`, `twitter` and `email`. |<br/>
> | open                                      | Boolean                                                                                  |<br/>
> | read                                      | Boolean                                                                                  |<br/>
> | state                                     | String                                                                                   |<br/>
> | waiting_since                             | Date (UNIX timestamp)                                                                    |<br/>
> | snoozed_until                             | Date (UNIX timestamp)                                                                    |<br/>
> | tag_ids                                   | String                                                                                   |<br/>
> | priority                                  | String                                                                                   |<br/>
> | statistics.time_to_assignment             | Integer                                                                                  |<br/>
> | statistics.time_to_admin_reply            | Integer                                                                                  |<br/>
> | statistics.time_to_first_close            | Integer                                                                                  |<br/>
> | statistics.time_to_last_close             | Integer                                                                                  |<br/>
> | statistics.median_time_to_reply           | Integer                                                                                  |<br/>
> | statistics.first_contact_reply_at         | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.first_assignment_at            | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.first_admin_reply_at           | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.first_close_at                 | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_assignment_at             | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_assignment_admin_reply_at | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_contact_reply_at          | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_admin_reply_at            | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_close_at                  | Date (UNIX timestamp)                                                                    |<br/>
> | statistics.last_closed_by_id              | String                                                                                   |<br/>
> | statistics.count_reopens                  | Integer                                                                                  |<br/>
> | statistics.count_assignments              | Integer                                                                                  |<br/>
> | statistics.count_conversation_parts       | Integer                                                                                  |<br/>
> | conversation_rating.requested_at          | Date (UNIX timestamp)                                                                    |<br/>
> | conversation_rating.replied_at            | Date (UNIX timestamp)                                                                    |<br/>
> | conversation_rating.score                 | Integer                                                                                  |<br/>
> | conversation_rating.remark                | String                                                                                   |<br/>
> | conversation_rating.contact_id            | String                                                                                   |<br/>
> | conversation_rating.admin_d               | String                                                                                   |<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Run Assignment Rules on a conversation
> You can let a conversation be automatically assigned following assignment rules.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The identifier for the conversation as given by Intercom.<br/>

### Redact a conversation part
> You can redact a conversation part or the source message of a conversation (as seen in the source object).<br/>
> <br/>
> >  Which parts and source messages can I redact?<br/>
> ><br/>
> > If you are redacting a conversation part, it must have a `body`.<br/>
> > If you are redacting a source message, it must have been created by a contact.<br/>
> > We will return a `conversation_part_not_redactable` error if these criteria are not met.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Manage a conversation
> You can close a conversation.<br/>
> You can snooze a conversation to reopen on a future date.<br/>
> You can open a conversation which is `snoozed` or `closed`.<br/>
> You can assign a conversation to an admin and/or team.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The identifier for the conversation as given by Intercom.<br/>

### Retrieve a conversation
> You can fetch the details of a single conversation.<br/>
> <br/>
> This will return a single Conversation model with all its conversation parts.<br/>
> <br/>
> >  Hard limit of 500 parts<br/>
> ><br/>
> > The maximum number of conversation parts that can be returned via the API is 500. If you have more than that we will return the 500 most recent conversation parts.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The id of the conversation to target<br/>
* `display_as` - _optional_ - Set to plaintext to retrieve conversation messages in plain text.<br/>

### List all data attributes
> You can fetch a list of all data attributes belonging to a workspace for contacts, companies or conversations.<br/>

*Tags:* `Data Attributes`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `model` - _optional_ - Specify the data attribute model to return.<br/>
    Possible values: contact, company, conversation.
* `include_archived` - _optional_ - Include archived attributes in the list. By default we return only non archived data attributes.<br/>

### Detach a contact from a group conversation
> You can add participants who are contacts to a conversation, on behalf of either another contact or an admin.<br/>
> <br/>
> >  Note about contacts without an email<br/>
> ><br/>
> > If you add a contact via the email parameter and there is no user/lead found on that workspace with he given email, then we will create a new contact with `role` set to `lead`.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `conversation_id` - _required_ - The identifier for the conversation as given by Intercom.<br/>
* `contact_id` - _required_ - The identifier for the contact as given by Intercom.<br/>

### Create a data attribute
> You can create a data attributes for a `contact` or a `company`.<br/>

*Tags:* `Data Attributes`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Attach a contact to a conversation
> You can add participants who are contacts to a conversation, on behalf of either another contact or an admin.<br/>
> <br/>
> >  Note about contacts without an email<br/>
> ><br/>
> > If you add a contact via the email parameter and there is no user/lead found on that workspace with he given email, then we will create a new contact with `role` set to `lead`.<br/>

*Tags:* `Conversations`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The identifier for the conversation as given by Intercom.<br/>

### Submit a data event
> You will need an Access Token that has write permissions to send Events. Once you have a key you can submit events via POST to the Events resource, which is located at https://api.intercom.io/events, or you can send events using one of the client libraries. When working with the HTTP API directly a client should send the event with a `Content-Type` of `application/json`.<br/>
> <br/>
> When using the JavaScript API, [adding the code to your app](http://docs.intercom.io/configuring-Intercom/tracking-user-events-in-your-app) makes the Events API available. Once added, you can submit an event using the `trackEvent` method. This will associate the event with the Lead or currently logged-in user or logged-out visitor/lead and send it to Intercom. The final parameter is a map that can be used to send optional metadata about the event.<br/>
> <br/>
> With the Ruby client you pass a hash describing the event to `Intercom::Event.create`, or call the `track_user` method directly on the current user object (e.g. `user.track_event`).<br/>
> <br/>
> | Type            | Description                                                                                                                                                                                                     | Example                                                                           |<br/>
> | :-------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------- |<br/>
> | String          | The value is a JSON String                                                                                                                                                                                      | `"source":"desktop"`                                                              |<br/>
> | Number          | The value is a JSON Number                                                                                                                                                                                      | `"load": 3.67`                                                                    |<br/>
> | Date            | The key ends with the String `_date` and the value is a [Unix timestamp](http://en.wikipedia.org/wiki/Unix_time), assumed to be in the [UTC](http://en.wikipedia.org/wiki/Coordinated_Universal_Time) timezone. | `"contact_date": 1392036272`                                                      |<br/>
> | Link            | The value is a HTTP or HTTPS URI.                                                                                                                                                                               | `"article": "https://example.org/ab1de.html"`                                     |<br/>
> | Rich Link       | The value is a JSON object that contains `url` and `value` keys.                                                                                                                                                | `"article": {"url": "https://example.org/ab1de.html", "value":"the dude abides"}` |<br/>
> | Monetary Amount | The value is a JSON object that contains `amount` and `currency` keys. The `amount` key is a positive integer representing the amount in cents. The price in the example to the right denotes EU349.99.          | `"price": {"amount": 34999, "currency": "eur"}`                                   |<br/>
> <br/>
> **NB: For the JSON object types, please note that we do not currently support nested JSON structure.**<br/>
> <br/>
> >  Lead Events<br/>
> ><br/>
> > When submitting events for Leads, you will need to specify the Lead's `id`.<br/>
> <br/>
> >  Metadata behaviour<br/>
> ><br/>
> > - We currently limit the number of tracked metadata keys to 10 per event. Once the quota is reached, we ignore any further keys we receive. The first 10 metadata keys are determined by the order in which they are sent in with the event.<br/>
> > - It is not possible to change the metadata keys once the event has been sent. A new event will need to be created with the new keys and you can archive the old one.<br/>
> > - There might be up to 24 hrs delay when you send a new metadata for an existing event.<br/>
> <br/>
> >  Event de-duplication<br/>
> ><br/>
> > The API may detect and ignore duplicate events. Each event is uniquely identified as a combination of the following data - the Workspace identifier, the Contact external identifier, the Data Event name and the Data Event created time. As a result, it is **strongly recommended** to send a second granularity Unix timestamp in the `created_at` field.<br/>
> ><br/>
> > Duplicated events are responded to using the normal `202 Accepted` code - an error is not thrown, however repeat requests will be counted against any rate limit that is in place.<br/>
> <br/>
> ### HTTP API Responses<br/>
> <br/>
> - Successful responses to submitted events return `202 Accepted` with an empty body.<br/>
> - Unauthorised access will be rejected with a `401 Unauthorized` or `403 Forbidden` response code.<br/>
> - Events sent about users that cannot be found will return a `404 Not Found`.<br/>
> - Event lists containing duplicate events will have those duplicates ignored.<br/>
> - Server errors will return a `500` response code and may contain an error message in the body.<br/>

*Tags:* `Data Events`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Update a data attribute
> You can update a data attribute.<br/>
> <br/>
> >  Updating the data type is not possible<br/>
> ><br/>
> > It is currently a dangerous action to execute changing a data attribute's type via the API. You will need to update the type via the UI instead.<br/>

*Tags:* `Data Attributes`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The data attribute id<br/>

### Create content data export
> To create your export job, you need to send a `POST` request to the export endpoint `https://api.intercom.io/export/content/data`.<br/>
> <br/>
> The only parameters you need to provide are the range of dates that you want exported.<br/>
> <br/>
> > Limit of one active job<br/>
> ><br/>
> > You can only have one active job per workspace. You will receive a HTTP status code of 429 with the message Exceeded rate limit of 1 pending message data export jobs if you attempt to create a second concurrent job.<br/>
> <br/>
> > Updated_at not included<br/>
> ><br/>
> > It should be noted that the timeframe only includes messages sent during the time period and not messages that were only updated during this period. For example, if a message was updated yesterday but sent two days ago, you would need to set the created_at_after date before the message was sent to include that in your retrieval job.<br/>
> <br/>
> > Date ranges are inclusive<br/>
> ><br/>
> > Requesting data for 2018-06-01 until 2018-06-30 will get all data for those days including those specified - e.g. 2018-06-01 00:00:00 until 2018-06-30 23:59:99.<br/>

*Tags:* `Data Export`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Create event summaries
> Create event summaries for a user. Event summaries are used to track the number of times an event has occurred, the first time it occurred and the last time it occurred.<br/>

*Tags:* `Data Events`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List all data events
> > <br/>
> ><br/>
> > Please note that you can only 'list' events that are less than 90 days old. Event counts and summaries will still include your events older than 90 days but you cannot 'list' these events individually if they are older than 90 days<br/>
> <br/>
> The events belonging to a customer can be listed by sending a GET request to `https://api.intercom.io/events` with a user or lead identifier along with a `type` parameter. The identifier parameter can be one of `user_id`, `email` or `intercom_user_id`. The `type` parameter value must be `user`.<br/>
> <br/>
> - `https://api.intercom.io/events?type=user&user_id={user_id}`<br/>
> - `https://api.intercom.io/events?type=user&email={email}`<br/>
> - `https://api.intercom.io/events?type=user&intercom_user_id={id}` (this call can be used to list leads)<br/>
> <br/>
> The `email` parameter value should be [url encoded](http://en.wikipedia.org/wiki/Percent-encoding) when sending.<br/>
> <br/>
> You can optionally define the result page size as well with the `per_page` parameter.<br/>

*Tags:* `Data Events`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `filter` - _required_
* `type` - _required_ - The value must be user<br/>
* `summary` - _optional_ - summary flag<br/>

### Cancel content data export
> You can cancel your job<br/>

*Tags:* `Data Export`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `job_identifier` - _required_ - job_identifier<br/>

### Download content data export
> When a job has a status of complete, and thus a filled download_url, you can download your data by hitting that provided URL, formatted like so: https://api.intercom.io/download/content/data/xyz1234.<br/>
> <br/>
> Your exported message data will be streamed continuously back down to you in a gzipped CSV format.<br/>
> <br/>
> >  Octet header required<br/>
> ><br/>
> > You will have to specify the header Accept: `application/octet-stream` when hitting this endpoint.<br/>

*Tags:* `Data Export`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `job_identifier` - _required_ - job_identifier<br/>

### List all live newsfeed items
> You can fetch a list of all news items that are live on a given newsfeed<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the news feed item which is given by Intercom.<br/>

### Create a message
> You can create a message that has been initiated by an admin. The conversation can be either an in-app message or an email.<br/>
> <br/>
> >  Sending for visitors<br/>
> ><br/>
> > There can be a short delay between when a contact is created and when a contact becomes available to be messaged through the API. A 404 Not Found error will be returned in this case.<br/>
> <br/>
> This will return the Message model that has been created.<br/>
> <br/>
> >  Retrieving Associated Conversations<br/>
> ><br/>
> > As this is a message, there will be no conversation present until the contact responds. Once they do, you will have to search for a contact's conversations with the id of the message.<br/>

*Tags:* `Messages`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Show content data export
> You can view the status of your job by sending a `GET` request to the URL<br/>
> `https://api.intercom.io/export/content/data/{job_identifier}` - the `{job_identifier}` is the value returned in the response when you first created the export job. More on it can be seen in the Export Job Model.<br/>
> <br/>
> >  Jobs expire after two days<br/>
> > All jobs that have completed processing (and are thus available to download from the provided URL) will have an expiry limit of two days from when the export ob completed. After this, the data will no longer be available.<br/>

*Tags:* `Data Export`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `job_identifier` - _required_ - job_identifier<br/>

### Create a news item
> You can create a news item<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a news item
> You can fetch the details of a single news item.<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the news item which is given by Intercom.<br/>

### Delete a news item
> You can delete a single news item.<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the news item which is given by Intercom.<br/>

### List all news items
> You can fetch a list of all news items<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a note
> You can fetch the details of a single note.<br/>

*Tags:* `Notes`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given note<br/>

### List all segments
> You can fetch a list of all segments.<br/>

*Tags:* `Segments`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `include_count` - _optional_ - It includes the count of contacts that belong to each segment.<br/>

### Update a news item

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the news item which is given by Intercom.<br/>

### Retrieve a segment
> You can fetch the details of a single segment.<br/>

*Tags:* `Segments`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identified of a given segment.<br/>

### List all newsfeeds
> You can fetch a list of all newsfeeds<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a newsfeed
> You can fetch the details of a single newsfeed<br/>

*Tags:* `News`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier for the news feed item which is given by Intercom.<br/>

### Create or update a tag, Tag or untag companies, Tag contacts
> You can use this endpoint to perform the following operations:<br/>
> <br/>
>   **1. Create a new tag:** You can create a new tag by passing in the tag name as specified in "Create or Update Tag Request Payload" described below.<br/>
> <br/>
>   **2. Update an existing tag:** You can update an existing tag by passing the id of the tag as specified in "Create or Update Tag Request Payload" described below.<br/>
> <br/>
>   **3. Tag Companies:** You can tag single company or a list of companies. You can tag a company by passing in the tag name and the company details as specified in "Tag Company Request Payload" described below. Also, if the tag doesn't exist then a new one will be created automatically.<br/>
> <br/>
>   **4. Untag Companies:** You can untag a single company or a list of companies. You can untag a company by passing in the tag id and the company details as specified in "Untag Company Request Payload" described below.<br/>
> <br/>
>   **5. Tag Multiple Users:** You can tag a list of users. You can tag the users by passing in the tag name and the user details as specified in "Tag Users Request Payload" described below.<br/>
> <br/>
> Each operation will return a tag object.<br/>

*Tags:* `Tags`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Create a phone Switch
> You can use the API to deflect phone calls to the Intercom Messenger.<br/>
> Calling this endpoint will send an SMS with a link to the Messenger to the phone number specified.<br/>
> <br/>
> If custom attributes are specified, they will be added to the user or lead's custom data attributes.<br/>

*Tags:* `Switch`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### List all tags
> You can fetch a list of all tags for a given workspace.<br/>

*Tags:* `Tags`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Delete tag
> You can delete the details of tags that are on the workspace by passing in the id.<br/>

*Tags:* `Tags`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given tag<br/>

### List subscription types
> You can list all subscription types. A list of subscription type objects will be returned.<br/>

*Tags:* `Subscription Types`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Find a specific tag
> You can fetch the details of tags that are on the workspace by their id.<br/>
> This will return a tag object.<br/>

*Tags:* `Tags`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given tag<br/>

### List all teams
> This will return a list of team objects for the App.<br/>

*Tags:* `Teams`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a team
> You can fetch the details of a single team, containing an array of admins that belong to this team.<br/>

*Tags:* `Teams`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - The unique identifier of a given team.<br/>

### Update a visitor
> Sending a PUT request to `/visitors` will result in an update of an existing Visitor.<br/>
> <br/>
> **Option 1.** You can update a visitor by passing in the `user_id` of the visitor in the Request body.<br/>
> <br/>
> **Option 2.** You can update a visitor by passing in the `id` of the visitor in the Request body.<br/>

*Tags:* `Visitors`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

### Retrieve a visitor with User ID
> You can fetch the details of a single visitor.<br/>

*Tags:* `Visitors`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `user_id` - _required_ - The user_id of the Visitor you want to retrieve.<br/>

### Delete a visitor
> You can delete a single visitor.<br/>

*Tags:* `Visitors`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - Id provided by Intercom.<br/>

### Retrieve a visitor with ID
> You can fetch the details of a single visitor.<br/>

*Tags:* `Visitors`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.
* `id` - _required_ - Id provided by Intercom.<br/>

### Convert a visitor
> You can merge a Visitor to a Contact of role type `lead` or `user`.<br/>
> <br/>
> >  What happens upon a visitor being converted?<br/>
> ><br/>
> > If the User exists, then the Visitor will be merged into it, the Visitor deleted and the User returned. If the User does not exist, the Visitor will be converted to a User, with the User identifiers replacing it's Visitor identifiers.<br/>

*Tags:* `Visitors`

#### Input Parameters
* `Intercom-Version` - _optional_
    Possible values: 1.0, 1.1, 1.2, 1.3, 1.4, 2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, Unstable.

## License

: intercom-connector<br/>
                    <br/>

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
