# ![LOGO](logo.png) groupalarm App API **flow**ground Connector

## Description

A generated **flow**ground connector for the groupalarm App API API (version 1.15.2).

Generated from: https://app.groupalarm.com/api/v1/app<br/>
Generated at: 2019-07-26T13:59:32+03:00

## API Description

The app service implements all app functions for GroupAlarm<br/>
<br/>
# Authentication<br/>
<br/>
<!-- ReDoc-Inject: <security-definitions> --><br/>

## Authorization

Supported authorization schemes:
- API Key
- API Key

## Actions

### List
> Returns all devices for queried owner<br/>

*Tags:* `device`

#### Input Parameters
* `owner_id` - _required_ - requested owner by using his userID<br/>
* `organization_id` - _optional_ - requesting organization, not required if user accesses his own resources<br/>

### Create
> Create a device configuration for specific user, used by our iOS / Android app<br/>

*Tags:* `device`

### Get
> Gets a device configuration<br/>

*Tags:* `device`

#### Input Parameters
* `deviceID` - _required_ - ID of a device configuration<br/>
* `organization_id` - _optional_ - requesting organization, not required if user accesses his own resources<br/>

### Update
> Updates an existing device configuration<br/>

*Tags:* `device`

#### Input Parameters
* `deviceID` - _required_ - ID of an existing device configuration<br/>
* `organization_id` - _optional_ - requesting organization, not required if user accesses his own resources<br/>

### Delete
> Delete an existing device configuration<br/>

*Tags:* `device`

#### Input Parameters
* `deviceID` - _required_ - ID of an existing device configuration<br/>
* `organization_id` - _optional_ - requesting organization, not required if user accesses his own resources<br/>

### GetDisabledOrganization
> Returns whether the given organization has disabled this way of alarming or not<br/>

*Tags:* `organizations`

#### Input Parameters
* `organization_id` - _required_ - requesting organization<br/>

### SetDisabledOrganization
> Sets whether the given organization has this way of alarming disabled or not<br/>

*Tags:* `organizations`

#### Input Parameters
* `organization_id` - _required_ - requesting organization<br/>

### Answered
> Sets a push's alarm answer<br/>

*Tags:* `push`

#### Input Parameters
* `token` - _required_ - confirmToken associated with this push<br/>
* `answer` - _required_ - answer given by the user (yes / no)<br/>

### Delivered
> Sets a push's status to delivered<br/>

*Tags:* `push`

#### Input Parameters
* `token` - _required_ - confirmToken associated with this push<br/>

## License

**flow**ground :- Telekom iPaaS / groupalarm-app-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
