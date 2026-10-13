TEAM B STAGE & OFFSTAGE WEBSITE — MOBILE STARTER
=================================================
Includes these independent lists:
- Senior Stage
- Senior Offstage
- Junior Stage
- Junior Offstage
- Sub Junior Stage
- Sub Junior Offstage
- General

Students and tick marks have been prefilled from the photos as far as they could be read. Some handwriting/ticks are ambiguous, so check the marks against the original paper. Event headings that are difficult to read are currently placeholders (“മത്സരം 1”, etc.) and can be renamed by the admin.

This package is NOT a live website yet. It needs Firebase setup and hosting.

FIREBASE SETUP:
1. Open https://console.firebase.google.com/ and create a project.
2. Project settings > General > Your apps > Add app > Web app. Copy firebaseConfig into index.html, replacing PASTE_ values.
3. Authentication > Sign-in method: enable Email/Password.
4. Authentication > Users: add the admin email/password, then copy the admin user's UID.
5. Create a Firestore database. Open Rules, paste firestore.rules, replace PASTE_ADMIN_USER_UID_HERE with the admin UID, then Publish.
6. Host index.html on a static host. GitHub Pages is free for a public repository; Firebase Hosting can also be used but the usual deploy flow uses Firebase CLI.
7. Public visitors can view the lists; only the configured admin UID can save changes.

Security: Firestore rules enforce write permission. Never put service-account credentials in the website.
