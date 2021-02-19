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

### Using HTML5 Storage
