# Beydex-OTA
Over the air updates for beydex native


1. Build the Update ZIP
Open your terminal in VSCode and run this custom command:

`npm run build:ota`

This will automatically compile your Next.js app and package it into a nice, neat update.zip file located in the root of your project folder.

2. Upload the ZIP to GitHub:

- Go to your repository on GitHub.com

- Go to Releases on the right side and click Draft a new release.

- Create a tag (like v1.0.1).

- Drag and drop your new update.zip file into the "Attach binaries" box at the bottom.

- Publish the release.

Once published, right-click the update.zip file in the release assets and select `Copy Link Address`.

3. Trigger the Update via Firebase:

- Go to your Firebase Console -> Remote Config.

- Edit the app_update_version parameter and change it to 1.0.1.

- Edit the app_update_url parameter and paste the GitHub link you copied in step 2.

- Click Publish Changes.