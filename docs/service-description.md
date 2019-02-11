# Happit Service Description

This document describes all major features of Happit. Happit can be used to train and support end users in the context of the web application to be more productive. There is no need to read the manual separately when support can be provided when using the application.

## What's new

Happspots can now be created in click away menus with limited features.

## System requirements

Supported browsers

- Edge
- Firefox
- Chrome
- Internet Explorer (some limitations apply)

## Features

### Happit switch

Happit switch is used to turn Happit on and off on the page. When switch is on Happspot icons are shown on web pages and Happspots with auto-open setting on will open automatically.

[Read more](./service-description/happit-switch.md)

### Happit content admin switch

Content admin switch is used to create new Happspots on web pages, see statistics and a list of Happspots in the application. When content admin switch is on user can hover on top of any element and using selector, red square, create a new Happspot or sequence by right clicking the element.

[Read more](./service-description/happit-content-admin-switch.md)

### Happspots

Happspots are icons in the web page which open by clicking or hovering it. Happspots are created next to UI elements in the web application to provide additional information for users how and when to use it. Happspots contain information such as title, content, image, embedded video or action link to guide users using the application. Content admins can create Happspots for end users to consume.

[Read more](./service-description/happspots.md)

### Multilanguage support

Multilanguage support provides content admins ability to serve content using the native language of users based on their browser language settings. Content can be created in original language and be translated manually and/or automatically to defined target languages.

Users can alternatively translate content from original language automatically to their native language.

Automatic translation uses Microsoft Azure Cognitive Services to translate the content into selected languages.

[Read more](./service-description/multilanguage-support.md)

### Statistics

Statistics give content admin a view of total number od active users, Happspots read count, most read and least read Happspots. By using statistics task pane content admins are able to find our situations where users need more guidance and which funcionalities are familiar for users.

[Read more](./service-description/statistics.md)

### Happspot list

Happspot list enables content admin to see all Happspots in the application in a single view. Content admin can filter Happspots by type, status and language to do actions like publish drafts more easily.

[Read more](./service-description/happspot-list.md)

### Browser extension

Happit browser extension can be used when Happit is needed without access to target system source code. With browser extension Happit is injected at browser side by the extension to enable same user experience after injection as in normal scenario where Happit is injected into the source code.

[Read more](./service-description/browser-extension.md)

### Admin portal

Admin portal is used by tenant admins to manage tenant where all Happit applications, users and Happspots are stored. Admin is able to manage tenant and application level settings to support various scenario and features such as Happspot colors, different types of web application (SharePoint, Dynamics 365, etc.)

[Read more]
