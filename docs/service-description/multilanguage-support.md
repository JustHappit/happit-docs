# Multilanguage support

Multilanguage support provides content admins ability to serve content using the native language of users based on their browser language settings. Content can be created in original language defined in admin portal and be translated manually and/or automatically to defined target languages.

Users can alternatively translate content from original language automatically to their native language.

Automatic translation uses Microsoft Azure Cognitive Services to translate the content into selected languages.

## Settings

- Tenant level languages are set in the admin portal. When set all application have translate functionality for content admins turned on.

- Automatic translation enables sending data to Azure Cognitive Services by content admins or end users to do automatic translation of the title and content of Happspot.

## Actions

- Content admins
  - When multiple languages have been set in admin portal content admins can translate the content to target languages.
  - § When automatic translation service has been turned on content admins can use automatic translation to translate set languages from original version
- Users
  - When browser language is set to other than original a translated version is shown automatically to the user if translated by content admin
  - When automatic translation service has been turned on and browser language is set to other than original user can use automatic translation to translate the content of the Happspot to language set by browser