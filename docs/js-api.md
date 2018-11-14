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
