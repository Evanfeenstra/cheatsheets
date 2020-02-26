# firebase

**how to `firebase init`:**

- Select the resources you want to use
  - Hosting (the actualy web host, you need this)
  - Firestore (realtime DB)
  - Storage (storing files)

- Public directory:
  - "build" (this is the directory that `create-react-app` builds into)

- Configure as a single-page app?
  - Yes!

- Overwrite the build/index.html?
  - No!

- Other questions, you can go with the defaults


### deployment

- make sure your logged in to firebase (`firebase login`)
- `npm run build`
- `firebase deploy`

### on the firebase console

- you can find your credentials in the "settings" menu, scroll down and click the "JSON" tab, which will give you a JS object that you can put in your db.js file.

- make sure to update your firebase rules files


