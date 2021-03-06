# Docusaurus Netlify CMS Starter

This is a starter website built using [Docusaurus 2](https://v2.docusaurus.io/), a modern static website generator, with Netlify CMS enabled.

### Pre-Req

Node.js version >= 12.13.0 or above (which can be checked by running node -v). You can use nvm for managing multiple Node versions on a single machine installed

Yarn version >= 1.5 (which can be checked by running yarn --version). Yarn is a performant package manager for JavaScript and replaces the npm client. It is not strictly necessary but highly encouraged.

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

### Run Commento(Comments Service)

```
$ docker-compose -f docker-compose.yml up
```

This command brings up the commento service on http://localhost:8080. Please sign up with test@testmail.com and a password. Then add a domain with http://localhost:3000/netifly-docusaurus. Customise the settings as you see fit. 

### Local Development

```
$ yarn start
```

This command starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.


### Test

Open http://localhost:3000/netifly-docusaurus/ for your website and http://localhost:3000/netifly-docusaurus/admin for the CMS. 

Notice changes will create/update files directly within your repo locally. 

Beyond this demo, the next step would be to update the static/admin/config.yml to remove local backend and use another provider(probably using [gotrue.js](https://github.com/netlify/gotrue-js))
