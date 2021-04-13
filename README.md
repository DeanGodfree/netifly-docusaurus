# Docusaurus Netlify CMS Starter

This is a starter website built using [Docusaurus 2](https://v2.docusaurus.io/), a modern static website generator, with Netlify CMS enabled.

### Installation

```
$ yarn
```

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Run CMS

```
$ npx netlify-cms-proxy-server
```

This command runs the CMS on port 8081 locally(make sure there are no conflicts)

### Local Development

```
$ yarn start
```

This command starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.


### Test

Open http://localhost:3000 for your website and http://localhost:3000/admin for the CMS. 

Notice changes will create/update files directly within your repo locally. 

Beyond this demo, the next step would be to update the static/admin/config.yml to remove local backend and use another provider(probably using [gotrue.js](https://github.com/netlify/gotrue-js))
