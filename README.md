# ![LOGO](logo.png) Semantria **flow**ground Connector

## Description

A generated **flow**ground connector for the Semantria API (version 4.0).

Generated from: https://api.apis.guru/v2/specs/semantria.com/4.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:58+03:00

## API Description

Semantria applies Text and Sentiment Analysis to tweets, facebook posts, surveys, reviews or enterprise content.

## Authorization

This API does not require authorization.

## Actions

### Remove items from blacklist

> This method removes certain blacklisted items by their values on Semantria side.

*Tags:* `Blacklist`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration blacklist items linked to.
* `content_type` - _required_

### Retrieve blacklisted items

> This method retrieves all backlisted items available on Semantria side.

*Tags:* `Blacklist`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration blacklist linked to.
* `content_type` - _required_

### Add items to blacklist

> This method adds new unique items to the backlist on Semantria side.

*Tags:* `Blacklist`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration blacklist linked to.
* `content_type` - _required_

### Update items in blacklist

> This method updates existing items by unique IDs in the backlist on Semantria side.

*Tags:* `Blacklist`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration blacklist linked to.
* `content_type` - _required_

### Remove user categories

> This method removes certain user categories by their IDs on Semantria side.

*Tags:* `Categories`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user categories linked to.
* `content_type` - _required_

### Retrieve user categories

> This method retrieves list of user categories available on Semantria side.

*Tags:* `Categories`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user categories linked to.
* `content_type` - _required_

### Add user categories

> This method adds user categories on Semantria side.

*Tags:* `Categories`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user categories linked to.
* `content_type` - _required_

### Updates user categories

> This method updates user categories by unique IDs on Semantria side.

*Tags:* `Categories`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user categories linked to.
* `content_type` - _required_

### Queue collection for analysis

> This method queues collection of documents onto the server for analysis. Queued collection of documents analyzes in common context as entire thing. If unique configuration ID provided, Semantria uses settings of that configuration during analysis, in opposite the primary configuration uses. Collection IDs are unique in scope of configuration. If the same ID appears twice, Semantria overrides existing collection with the new Data

*Tags:* `ProcessingCollections`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `content_type` - _required_

### Retrieve collections analysis

> This method retrieves analysis results for processed collections from Semantria. FAILED collections will have FAILED status in response. Semantria responds with limited amount of results per API call. If configuration ID provided, Semantria responds with the collections, which were queued using the same configuration ID, in opposite Primary configuration uses.

*Tags:* `ProcessingCollections`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `content_type` - _required_

### Cancel collection analysis

> This method cancels collection analysis by unique ID on Semantria side if it is waiting for analysis in queue.

*Tags:* `ProcessingCollections`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `collection_id` - _required_ - Collection ID
* `content_type` - _required_

### Retrieve collection analysis or its status in queue

> This method retrieves analysis results for documents collection by its unique ID or the collection's status in queue if it did not analyzed yet. Semantria guarantees delivering of all collections back to the client even if they FAILED on Semantria side due to some reason.

*Tags:* `ProcessingCollections`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `collection_id` - _required_ - Collection ID
* `content_type` - _required_

### Remove user configurations

> This method removes certain configuration by unique ID on Semantria side.

*Tags:* `Configuration`

#### Input Parameters
* `content_type` - _required_

### Retrieve user configurations

> This method retrieves all user configurations available on Semantria side.

*Tags:* `Configuration`

#### Input Parameters
* `content_type` - _required_

### Create user configurations

> This method creates configurations on Semantria side.

*Tags:* `Configuration`

#### Input Parameters
* `content_type` - _required_

### Update user configurations

> This method updates specific configurations by unique IDs on Semantria side.

*Tags:* `Configuration`

#### Input Parameters
* `content_type` - _required_

### Queue document for analysis

> This method queues document onto the server for analysis. Queued document analyzes individually and will have its own set of results. If unique configuration ID provided, Semantria uses settings of that configuration during analysis, in opposite the primary configuration uses. Document IDs are unique in scope of configuration. If the same ID appears twice, Semantria overrides existing document with the new Data.

*Tags:* `ProcessingDocuments`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `content_type` - _required_

### Queue batch of documents for analysis

> This method queues batch of documents for analysis. The rules are the same as for single document mode but here the documents ordered into the batch.

*Tags:* `ProcessingDocuments`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `content_type` - _required_

### Retrieve documents analysis

> This method retrieves analysis results for processed documents from Semantria. FAILED documents will have FAILED status in response. Semantria responds with limited amount of results per API call. If configuration ID provided, Semantria responds with the document, which were queued using the same configuration ID, in opposite Primary.

*Tags:* `ProcessingDocuments`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `content_type` - _required_

### Cancel document analysis

> This method cancels document analysis by unique ID on Semantria side if it is waiting for analysis in queue.

*Tags:* `ProcessingDocuments`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `document_id` - _required_ - Document ID
* `content_type` - _required_

### Retrieve document analysis or its status in queue

> This method retrieves analysis results for the single document by its unique ID or the document's status in queue if it did not analyzed yet. Semantria guarantees delivering of all documents back to the client even if they FAILED on Semantria side due to some reason.

*Tags:* `ProcessingDocuments`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration used for analysis.
* `document_id` - _required_ - Document ID
* `content_type` - _required_

### Remove user entities

> This method removes certain user entities by their names on Semantria side.

*Tags:* `Entities`

#### Input Parameters
* `content_type` - _required_

### Retrieve user entities

> This method retrieves list of user entities available on Semantria side.

*Tags:* `Entities`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user entities linked to.
* `content_type` - _required_

### Add user entities

> This method adds user entities on Semantria side.

*Tags:* `Entities`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user entities linked to.
* `content_type` - _required_

### Update user entities

> This method updates user entities by unique IDs on Semantria side.

*Tags:* `Entities`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration user entities linked to.
* `content_type` - _required_

### Retrieve supported features

> This method returns list of supported features per languages supported by Semantria API. Let the users know about API capabilities.

*Tags:* `Features`

#### Input Parameters
* `language` - _optional_ - Filter features by specified language
* `content_type` - _required_

### Remove sentiment-bearing phrases

> This method removes certain sentiment-bearing phrases by their names on Semantria side.

*Tags:* `Phrases`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration phrases linked to.
* `content_type` - _required_

### Retrieve sentiment-bearing phrases

> This method retrieves list of sentiment-bearing phrases available on Semantria side.

*Tags:* `Phrases`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration phrases linked to.
* `content_type` - _required_

### Add sentiment-bearing phrases

> This method adds sentiment-bearing phrases on Semantria side.

*Tags:* `Phrases`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration phrases linked to.
* `content_type` - _required_

### Updates sentiment-bearing phrases

> This method updates sentiment-bearing phrases by unique IDs on Semantria side.

*Tags:* `Phrases`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration phrases linked to.
* `content_type` - _required_

### Remove queries

> This method removes certain queries by their IDs on Semantria side.

*Tags:* `Queries`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Retrieve queries

> This method retrieves list of queries available on Semantria side.

*Tags:* `Queries`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Add or update queries

> This method adds queries on Semantria side.

*Tags:* `Queries`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Update queries

> This method updates queries by unique IDs on Semantria side.

*Tags:* `Queries`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Retrieve usage statistics

> This method retrieves overall and per configuration usage statistics for specific timeframe. Statistics ordered per available configurations. Available interval values are current <b>hour</b>, <b>day</b>, <b>week</b>, <b>month</b> and <b>year</b>.

*Tags:* `Statistics`

#### Input Parameters
* `config_id` - _optional_ - Configuration identifier for usage statistics retrieving.
* `interval` - _optional_ - Hour, Day, Week, Month, Year values are supported.
* `content_type` - _required_

### Retrieve API status

> This method retrieves API status information such as the app version, current API version, supported languages and encodings, the overall service status, etc.

*Tags:* `Status`

#### Input Parameters
* `content_type` - _required_

### Retrieve subscription details

> This method retrieves user's subscription details that consist of the list of allowed features, configured limits and options on Semantria side.

*Tags:* `Subscription`

#### Input Parameters
* `content_type` - _required_

### Remove taxonomy nodes

> This method removes certain taxonomy nodes by their IDs on Semantria side.

*Tags:* `Taxonomy`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Retrieve taxonomy

> This method retrieves list of taxonomy available on Semantria side.

*Tags:* `Taxonomy`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration taxonomy linked to.
* `content_type` - _required_

### Add taxonomy nodes

> This method adds taxonomy nodes on Semantria side.

*Tags:* `Taxonomy`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

### Update taxonomy nodes

> This method updates taxonomy nodes on Semantria side.

*Tags:* `Taxonomy`

#### Input Parameters
* `config_id` - _optional_ - Identifier of configuration queries linked to.
* `content_type` - _required_

## License

**flow**ground :- Telekom iPaaS / semantria-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
