# nuxt-firebase

universal nuxt project distributed to firebase hosting and firebase functions

## Pre requirements

- Install [firebase tools] [firebase-tools].
  > npm i -g firebase-tools
- Create a firebase project in [Firebase Console] [[firebase-console]] and write the project id under the project item of `.firebaserc`.

```json
    {
        "projects": {
            "default": "your-firebase-project-id"
        }
    }
```

- Log in to firebase from the console.

> firebase login

## Development

When developing nuxt pages, run the `npm run dev` command under the` src / `directory to develop rapidly.
> npm run dev

To verify that the firebase functions are working before deployment, emulate the functions through the `firebase serve` command in the project root directory.
> firebase serve --only functions

When deploying after development, deploy with the `firebase deploy` command
> firebase deploy -m "first release"

[firebase-tools]: https://firebase.google.com/docs/cli/
[firebase-console]: https://console.firebase.google.com/u/0/