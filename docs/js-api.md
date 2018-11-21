# Happit JS API

All the methods are accessible through global object called `Happit`.

Because Happit is loaded asynchronously in the application, you must wait for the API to be available.  
For example something like this:

```javascript
const waitHappit = setInterval(() => {
    if (typeof Happit === 'undefined') return
    clearInterval(waitHappit)

    doYourMagicWithHappit()
}, 200)
```

---

## setTheme(options: object)

All options are optional and if omitted, default Happit theme is used on those parts.

Notes:

* Colors must be set as hex, rgb(), or rgba().
* You can add as many fonts as you want, just separate them with commas

```javascript
Happit.setTheme({
    // background color used basically everywhere
    // default: #FFF
    backgroundColor: string,
    // text color used in all typography elements
    // default: #000
    textColor: string,
    // color used to bring contrast in some elements (e.g. backgrounds and buttons)
    // default: #00aeff
    contrastColor: string,
    // text color used in all elements which have the contrast color as background
    // default: #FFF
    contrastTextColor: string,
    /*
        Font to be used everywhere.
        Actual font files and font-face definitions must be available in the application where Happit is used.

        Note: Happit default fonts will be used as fallback
    */
    // default: '"Roboto", "Helvetica", "Arial", sans-serif'
    fontFamily: string,

    // Overrides are for overriding the main theme in certain elements
    // default: not set
    overrides: {
        // Happspot callout
        callout: {
            // background color used on title area
            titleBackgroundColor: string,
            // text color used in title area
            titleTextColor: string,
            // background color used on content area
            backgroundColor: string,
            // text color used in content area
            textColor: string
        }
    }
})
```
