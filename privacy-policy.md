# Nerptify Privacy Policy

**Effective date:** 9 October 2026  
**App:** Nerptify (Android package `com.nerptify`; also available for Linux and Windows)  
**Developer:** Michael Oktavianus  
**Contact:** michaelokta555@gmail.com

Nerptify is a music player for music files you own. It has no account, no advertising, no analytics and no tracking, and it doesn't send any information about you or your use of the app to the developer or anyone else.

## What Nerptify stores, and where

Everything Nerptify keeps stays **on your device**:

- **Your music folders.** On Android this is Nerptify's own folder (`Android/data/com.nerptify/files/Music`) plus any music folder you pick. Nerptify reads your songs there and writes only what you ask it to: playlists and their covers, song details (title, artist, album and the like) and a cover picture you choose, written into the song file, and lyrics you edit, saved as a `.lrc` file next to the song. It never changes the music itself.
- **A library database** in the app's private storage, built from your music files: song details, cover pictures, lyrics you add, and your playlists.
- **Your settings and what was playing** (volume, the queue, the position in the current song), so the app can pick up where you left off.
- **A trash folder** in the app's private storage, holding older copies of files that "Fetch" replaced, for 30 days, so you can restore them. (Older copies that "Upload" replaced are kept the same way in a `.nerptify-trash` folder in your Google Drive.)

None of this is uploaded anywhere by Nerptify. Uninstalling the app deletes all of it, including Nerptify's own music folder on Android.

## Google Drive ("Upload" and "Fetch"), only if you use it

If you choose to connect Google Drive, Nerptify can copy music between your device and a folder in **your own** Google Drive, but only when you press **Upload** or **Fetch**. It never syncs in the background.

- The transfer is done by [rclone](https://rclone.org), an open-source tool bundled with the app, which talks **directly** between your device and Google. Nothing passes through any server run by the developer.
- Signing in happens in your web browser on Google's own page. The resulting access permission is stored only on your device, in the app's private storage, and is used only to read and write the Drive folder you sync with.
- Only files in your music folder and the Drive folder you choose are transferred.
- You can disconnect at any time with **Disconnect** in Settings → Music sync, by uninstalling the app, or by removing Nerptify/rclone's access in your Google Account settings (<https://myaccount.google.com/permissions>).

Google's handling of your Drive data is covered by [Google's Privacy Policy](https://policies.google.com/privacy).

## Android permissions

| Permission | Why |
|---|---|
| Internet | Only for Upload and Fetch (Google Drive), and for the app talking to its own built-in music server on the device (`127.0.0.1`), which is how songs are played. |
| Music and audio, photos and images | To read songs and folder cover pictures in music folders you pick. |
| Notifications | To show the playback notification with play/pause and next/previous controls, and the "Fetching music…" notification during sync. |
| Foreground service (media playback, data sync) | To keep music playing, and an Upload/Fetch or Google sign-in running, while the screen is off or another app is open. |

Nerptify does not ask for your location, contacts, camera or microphone.

## Data sharing and selling

Nerptify does not collect personal data, so it shares or sells none. No third-party libraries for advertising, analytics or crash reporting are included.

## Children

Nerptify is not directed at children and collects no data from anyone, children included.

## Changes

If this policy changes, the new version will be published at this address with a new effective date.

## Contact

Questions about this policy: michaelokta555@gmail.com

