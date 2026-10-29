# Magic Buttons

One-click buttons that type your saved text (replies, addresses, signatures, code snippets) into whatever you're working in.

- **Desktop app:** a small floating window. Click a button and its text is pasted into the app you were just using.
- **Chrome extension:** the same buttons in Chrome's side panel and in the right-click menu of any text field. It syncs your profiles with the desktop app.

**Downloads:** [latest release](https://github.com/kmlpandey77/magic-buttons-releases/releases/latest)

## Desktop app

Windows only for now.

1. From the [latest release](https://github.com/kmlpandey77/magic-buttons-releases/releases/latest), download the file ending in `_x64-setup.exe` (or the `.msi`) and run it.
2. Open **Magic Buttons**. It starts a 14-day trial; enter a license key under **Settings → License…**.

The app checks for updates when it starts and offers to install them.

## Chrome extension

The extension isn't on the Chrome Web Store yet, so you load it yourself in Developer mode. It works together with the desktop app, which has to be installed, opened at least once, and licensed (or in its trial).

### Install

1. Install the desktop app (above) and **open it once**. This registers it with Chrome.
2. From the [latest release](https://github.com/kmlpandey77/magic-buttons-releases/releases/latest), download `magic-buttons-extension-<version>.zip`.
3. Extract it. You get a folder called `magic-buttons-extension`. **Move that folder somewhere permanent**, e.g. `Documents\magic-buttons-extension`. Chrome loads the extension from this folder every time it starts, so don't delete it or leave it in Downloads.
4. In Chrome, open `chrome://extensions`.
5. Turn on **Developer mode** (switch in the top-right corner).
6. Click **Load unpacked** and select the `magic-buttons-extension` folder (the one that contains `manifest.json`).
7. Click the puzzle-piece icon in Chrome's toolbar and **pin** Magic Buttons.

Chrome may show a "Disable developer mode extensions" notice when it starts. Click **✕** (not *Disable*) to keep the extension running.

### Use

- **Side panel:** click the Magic Buttons toolbar icon. Click into a text field on the page, then click a button: its text is typed where your cursor was.
- **Right-click menu:** right-click in any text field → **Magic Buttons** → pick a button.
- Add, edit and reorder buttons in the side panel just like in the desktop app (right-click a button for Edit, Duplicate, Delete, Move).
- The **link icon** in the panel's footer shows the connection to the desktop app. When it's blue, profiles sync both ways within a second or so. Hover over it to see why if it isn't.

The extension can't type into Chrome's own pages (`chrome://…`) or the Chrome Web Store. Some editors that handle typing themselves, like Google Docs, may not accept the text; use the desktop app there.

### Update

When a new release is out:

1. Download the new `magic-buttons-extension-<version>.zip` and extract it.
2. **Replace the contents** of your existing `magic-buttons-extension` folder with the new files (delete the old files in it, then copy the new ones in). Keep the same folder location.
3. Open `chrome://extensions` and click the **reload** icon (↻) on the Magic Buttons card.

The version number on the card should now match the release. Your buttons are kept.

Keep the desktop app updated too: the extension expects the desktop app from the same release or newer.

**Don't click "Remove"** to update. Removing the extension deletes the buttons stored in Chrome. They come back from the desktop app once it's linked again, but replacing the files and reloading is simpler.

### Troubleshooting

| What you see | What to do |
| --- | --- |
| "Desktop app not found" | Install the desktop app and open it once, then click **Retry** in the panel. |
| "Open the Magic Buttons desktop app once…" | Open the desktop app, then click **Retry**. |
| "Your trial has ended" / "Your license has expired" | Enter a license key in the desktop app under **Settings → License…**. The extension picks it up within a few seconds. |
| "Click into a text field on the page first" | Click into the field you want to type in, then press the button again. |
| The extension disappeared after a Chrome restart | The `magic-buttons-extension` folder was moved or deleted. Put it back (or extract it again) and **Load unpacked** again. |
