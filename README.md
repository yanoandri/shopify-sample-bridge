# Shopify App Node - Tutorial

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE.md)

This branch contains one of the steps for the [Build a Shopify app with Node and React](https://developers.shopify.com/tutorials/build-a-shopify-app-with-node-and-react) tutorial (which i completed because they only give the template only).

## Configuration
1. Copy `.env.example` into `.env` file
2. Enter your shopify app credentials
   1. SHOPIFY_API_KEY = will be your client api key
   2. SHOPIFY_API_SECRETS = will be your secret api key
   3. SHOPIFY_API_SCOPES = your desirable scopes of the apps
   4. SHOPIFY_APP_URL = your secure url from `.ngrok` (see Shopify Configuration below)
   
## Installation 

```
npm install
```

run the projects :

```
npm run dev
```

## Shopify configuration

You can use [ngrok](https://ngrok.com/) to connect this repository to your shopify app
1. Run `./ngrok http 3000`
2. Go to your desire shopify public app
3. Choose App Setup
4. Copy the secure url from ngrok into "App Url"
5. Copy url to "Allowed Redirection URL(s)" by adding `/auth/callback`
6. Save it
7. Go back to your shopify public app main page and you can proceed to test the app into your desire store