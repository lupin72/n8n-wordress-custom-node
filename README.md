![Banner image](https://user-images.githubusercontent.com/10284570/173569848-c624317f-42b1-45a6-ab09-f0ea3c247648.png)

# n8n-nodes-wordpress-cpt

Custom n8n node to interact with WordPress Custom Post Types (CPTs) via the REST API.

## Prerequisites

You need the following installed on your development machine:

* [git](https://git-scm.com/downloads)
* Node.js and npm. Minimum version Node 20. You can find instructions on how to install both using nvm (Node Version Manager) for Linux, Mac, and WSL [here](https://github.com/nvm-sh/nvm). For Windows users, refer to Microsoft's guide to [Install NodeJS on Windows](https://docs.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows).
* Install n8n with:
  ```
  npm install n8n -g
  ```
* Recommended: follow n8n's guide to [set up your development environment](https://docs.n8n.io/integrations/creating-nodes/build/node-development-environment/).

## Features

- Create, get, update, delete posts of any post type
- Dynamically loads available post types from `/wp-json/wp/v2/types`
- Supports categories, tags, authors, and template selection
- Compatible with Elementor templates
- Uses `wordpressApi` credentials (Basic Auth, OAuth2, or JWT)

## Operations

- **Create** CPT post
- **Get** a CPT post by ID
- **Get Many** CPT posts (with filters)
- **Update** a CPT post
- **Delete** a CPT post
