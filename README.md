
# svelte boilerplate app

This boilerplate svelte app is customized with a few notable changes:  

### Build files are nested in `/static/` folder
Build files are nested in `/public/static/` folder instead of `/public/` and the links in `index.html` follows accordingly. This is to allow backends to serve svelte frontend easily in dedicated `/static/` folders that are meant for static assets.

### `svelte-routing` Router
`svelte-routing` package is included as the choice of router for this boilerplate. See [link](https://github.com/EmilTholin/svelte-routing "https://github.com/EmilTholin/svelte-routing")

### Single-page app mode

SPA mode activated by default in this template  
```js
"start": "sirv public --single"
```
This allows sirv to respond to any direct request to the routes and will serving up the correct content upon direct request.
