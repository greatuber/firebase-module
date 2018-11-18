# Nuxt-Fire

> Easily intergrate Firebase into your Nuxt 2 project.

## Demo

https://github.com/lupas/nuxt-fire-demo

## Requirements

Make sure to have Nuxt 2+ installed:

- Nuxt.js >= 2.x

## Install

```bash
npm i nuxt-fire
```

## Setup

Add the below code to **nuxt.config.js**.

```js
modules: [
    [
      'nuxt-fire',
      {
        config: {
          apiKey: '<apiKey>',
          authDomain: '<authDomain>',
          databaseURL: '<databaseURL>',
          projectId: '<projectId>',
          storageBucket: '<storageBucket>',
          messagingSenderId: '<messagingSenderId>'
        }
      }
    ]
  ],
```

## Options

##### useOnly

- type: Array<string>
- default: null
- example: ['']

##### config

Your firebase config snippet. You can retrieve this from your Firebase project overview page:
https://console.firebase.google.com/project/your-project-id/overview

## Usage

You can access the various Firebase services with **\$foo** in almost any context using `app.$foo` or `this.$foo`, including store actions. Make sure to replace the _foo_ with a shortcut from the table below.

Services supported by nuxt-fire so far:

| Firebase Service  | Shortcut        |
| ----------------- | --------------- |
| Authentication    | \$fireAuth      |
| RealTime Database | \$fireDb        |
| Firestore         | \$fireStore     |
| Storage           | \$fireStorage   |
| Functions         | \$fireFunctions |

See [Firebase's official docs](https://firebase.google.com/docs/) for more usage information.

### Examples

(tbd)

Check out the [Demo](https://github.com/lupas/nuxt-fire-demo) project for example code.
