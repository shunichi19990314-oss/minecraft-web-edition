# Minecraft Web Edition

A Japanese-language voxel sandbox game built with React, TypeScript, Three.js, and Vite.

## Requirements
- Node.js 22 or later
- npm 10 or later

## Local development
```sh
npm install
npm run dev
```

## Production build
```sh
npm install
npm run build
```

Vite outputs the production site to `dist/`.

## Render deployment
This repository stores the application source in the compressed `source.parts/` archive. The Render Static Site build command reconstructs the project and builds it:

```sh
cat source.parts/*.b64 | base64 -d | tar -xz
npm install --no-audit --no-fund
npm run build
```

Publish directory: `dist`
