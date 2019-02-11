# Happspots

Happspots can be created to majority of UI elements in web pages. When content admin switch is on you can select an element on the page by hovering and right clicking the element. Red square will show selected element. Happspots store the HTML element data such as page URL, HTML element ID, CSS classes and DOM structure information to locate right element on a page. Happit does not store any data from the page visible to users.

You can create

- normal Happspot,
- sequence of Happspots or
- image Happspot (if target element is an image)
- normal Happspot with limited features on click away menus

## Content

Title of the Happspot is required and will be shown also on a tooltip.

Content is shown below the title.

Content can be modified with font settings and paragraph settings.

- Font settings:

  - Bold
  - Italic
  - Underline
- Paragraph settings:
  - List
  - Numbered list
  - Line break

Additionally content can be

- Image URL to show single image or gif animation
- Embed code to show e.g. Office document, media file such as Microsoft Stream or YouTube video. (Feature not available in Happspot in click away menus)
- Action link to external resource  (Feature not available in Happspot in click away menus)

Title of the sequence (if sequence was created).

- Title will be shown for users in sequence next to Happspot order number

## Settings

Color of the Happspot icon. Can be managed in admin portal to set brand colors

- #00AEFF - Happit blue (default)
- #FFFFFF - White
- #000000 - Black

Width of the Happspot

- Auto (max 720 px wide)
- Small (340 px wide)
- Medium (540 px wide)
- Large (720 px wide)

Position - where Happspot content is located relative to the icon

- Top
- Bottom
- Left
- Right
- Top left
- Top right
- Bottom left
- Bottom right

Pinned - Happspot stays open and cannot be bypassed by clicking the page behind (backdrop) but it does not restrict using features of the page. Can be used e.g. when having guidelines in Happspot howto fill out a form or use certain functionality in the page.

Auto-open - Happspot automatically opens when user enters the page and Happit is turned on

Global - Happspot icon is shown always when same element is found on the page even in different URL. This might cause issues and should be used with active testing.

## Actions

For content admins

- Preview - preview how the Happspot looks before saving or publishing
- Save - save a draft version without publishing e.g. when making changes.
- Publish- publish Happspot to be visible for all users
- Delete - delete existing Happspot
- Translate - if additional languages set in the admin portal shown to enable manual translation for configured languages.
- Get translation - when translating content you can use Microsoft Azure Cognitive Services to get initial translation for your original content
- Add new Happspot to the sequence - when creating a sequence you can add new Happspots from the sequence toolbar
- Move next or previous in sequence - in sequence toolbar you can review the whole sequence by moving next or previous
- Order Happspots in sequence - in sequence toolbar you can change the order of Happspots

For users

- Got it! - Close the Happspot or move to next if sequence
- Translate - for end user possibility to translate content from original to version set in browser language
- Show original - shows original version in default language set on Happit
