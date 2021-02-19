# Class 13 Reading Notes - Local Storage

## The Past, Present, and Future of Local Storage for Web Applications

- Native client apps have an advantage over web apps because of local storage

- If native client happs need local storage, you can embed your own database, invent your own file format, or any number of solutions

- Cookies were used for web applications to store small amounts of data. But they had their disadvantages

## HTML5 Storage

- Web Storage ... a way for web pages to store name key/vaule pairs locally within the client web browser.
- Data stays even after you navigate from the website, close your browser, etc.
- Pretty much ever browser supports HTML5 Storage

- You can access HTML5 Storage through **localStorage** object in JavaScript

```` javascript
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
````

- You can also use **Modernizer** to detect support for HTML5 storage

```` javascript
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
````

### Using HTML5 Storage

- HTML5 Storage is based on named key/value pairs
  - data is stored on a named key
  - data can be retrieved with the key
  - key is always a string -- use things like `parseInt()` or `parseFloat()` to coerce data

- methods to use
  - `setItem()` - named key that already exists will silently overwrite the previous value
  - `getItem()`
  - `removeItem()`

- if you want to keep track of when storage area changes, you can use the *storage* event
