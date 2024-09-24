![SvelteKitXWordPress](static/readme-banner.png)

# SvelteKit with WordPress starter

<div>
  <img src="https://img.shields.io/badge/Svelte-orange?style=for-the-badge&logo=svelte&logoColor=white" alt="svelte">
  <img src="https://img.shields.io/badge/Typescript-blue?style=for-the-badge&logo=typescript&logoColor=white" alt="typescript">
  <img src="https://img.shields.io/badge/TailwindCSS-blue?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="tailwindcss">
  <img src="https://img.shields.io/badge/WordPress-gray?style=for-the-badge&logo=wordpress&logoColor=white" alt="wordpress">
  <img src="https://img.shields.io/badge/Docker-blue?style=for-the-badge&logo=docker&logoColor=white" alt="wordpress">
  <img src="https://img.shields.io/badge/Houdini-gray?style=for-the-badge&logoColor=white" alt="houdini">
  <img src="https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white" alt="houdini">
</div>

## Installation

```bash
docker compose up -d --build
```

It will start 2 servers. One for the WordPress app and the other for the client part with SvelteKit.

- `localhost` - WordPress

- `localhost:3000` - SvelteKit

Once that is done, go to `localhost/wp-admin` and follow the WordPress configuration instructions. Then, install and active the plugin named `WPGraphQL`.

Last step, go to `WPGraphQL` settings and check `Enable GraphQL Debug Mod`.

This plugin will allows your SvelteKit app to communicate with the WordPress app and get the data from it thanks to the Houdini GraphQL Client.