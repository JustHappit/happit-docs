# Happit data transfer

All the data transferred between the client and the servers are described here.

## Common

- Authorization token is sent in HTTP header of every request (except the authentication request)

## Authentication

### End users

To authenticate end users, in addition to the user identity (e.g. email address) we are using globally unique identifiers of the tenant and application.

### Content admins

To authenticate content admins we are using same information as for the end user authentication.

Paths:

- `/api/Authentication`

[See data models](./data-transfer/authentication.md)

## Happspots and sequences

### Read

All Happspots created for the application

*Only required data to show the Happspots in correct places with given content.*

### Write

Data given by the user is sent on these events

- Create a Happspot (save/publish)
- Modify a Happspot (save/publish)
- Delete a Happspot
- Click on "Got it!"
- Create a sequence (save/publish)
- Update a sequence (save/publish)

Paths:

- `/api/Hotspot`
- `/api/HotspotVersion`
- `/api/Sequence`

[See data models](./data-transfer/happspot.md)

## User requests

### Read

- Content admins: All user requests created for the application
- Users: All user requests created by themselves for the application

*Only required data to show the user requests in correct places with given content.*

### Write

Data given by the user is sent on these events

- Create an user request
- Modify an user request
- Delete an user request
- Promote an user request

Paths:

- `/graphql`

[See data models](./data-transfer/user-request.md)

## Settings

There's only read operations related to settings. These are the settings configured on tenant and application level in Happit Portal.

Paths:

- `/api/Settings`

[See data models](./data-transfer/settings.md)

## Statistics

There's only read operations related to statistics. Sum statistics of certain performance indicators. Does not include any user specific information.

Paths:

- `/graphql`

[See data models](./data-transfer/statistics.md)

## Translations

There's only read operations related to automatic translations. Users can use automatic translation depending on language settings of the application (in Happit Portal). **Title** and **content** of the Happspot is sent to Azure Cognitive Services to get the translations.

- `/graphql`

[See data models](./data-transfer/translations.md)

## Diagnostics

There's only write operations related to diagnostics. In case of certain errors, error descriptions are sent. Does not include any user specific information.

Paths:

- `/graphql`

[See data models](./data-transfer/diagnostics.md)

## Injection endpoint

There's only read operations related to injection script. Injection endpoint is the main entry point for Happit. It is added by system administrators or by the Happit browser extension. The address contains only the globally unique application identifier and no other information is passed to it.

Paths:

- `/inject/{application identifier}`

Contains JavaScript code
