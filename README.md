# NAKRI x OG — Music Website

A stylish, responsive music-listening website that can be hosted on **GitHub Pages**. Visitors can listen to songs, search the library, skip tracks, and control volume. There is no upload button for visitors.

## Folder layout

```text
NAKRI_x_OG_Music_Website/
├── index.html
├── style.css
├── app.js
├── songs.json
├── songs/
│   ├── PUT YOUR MP3 FILES HERE.txt
│   └── example-song.mp3        (your own file goes here)
└── thumbnails/
    ├── PUT YOUR PNG COVERS HERE.txt
    └── example-song.png        (your own cover goes here)
```

## Add a song (easy method)

1. Put the MP3 in the `songs` folder.
2. Put its PNG/JPG/WebP cover image in `thumbnails`.
3. Open `songs.json` with Notepad.
4. Add an entry for the song. The `file` and `cover` paths must match the names exactly, including spaces, capital letters and file extensions.

Example:

```json
[
  {
    "title": "Night Drive",
    "artist": "NAKRI x OG",
    "file": "songs/night-drive.mp3",
    "cover": "thumbnails/night-drive.png",
    "duration": "MP3"
  },
  {
    "title": "Blue Sky",
    "artist": "OG",
    "file": "songs/blue-sky.mp3",
    "cover": "thumbnails/blue-sky.jpg",
    "duration": "MP3"
  }
]
```

**Important:** This starter uses a small `songs.json` list. Adding files to the folders alone does not automatically make them appear; edit `songs.json` for each track. This is because a static GitHub Pages website cannot scan its folders automatically. The player reads the cover path you give it, so each track can have its own thumbnail.

### Naming tip

Use simple filenames without spaces, for example:
- `songs/my-new-song.mp3`
- `thumbnails/my-new-song.png`

The MP3 and cover do not technically need matching filenames, but using the same base name makes it easier.

## Publish on GitHub Pages

1. Sign in to GitHub and create a **public** repository, for example `nakri-og-music`.
2. Extract this ZIP on your Windows computer.
3. Upload the contents inside `NAKRI_x_OG_Music_Website` to the repository root. Make sure `index.html` is at the root, not inside another nested folder.
4. Open the repository **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then save.
7. Wait for GitHub Pages to publish your site. The Pages section will show the website address.

## Update your music later

Add the MP3 and cover, edit `songs.json`, then upload/commit the changed files to GitHub. GitHub Pages will update the site after the commit is published.

## Please note

- GitHub Pages is static hosting: there is no secure admin login or in-browser song upload in this starter. Only people with repository write access can change the website files.
- Large audio files can hit GitHub's file-size limits or make the repository very large. Check GitHub's current limits before uploading many or very large songs.
- Upload only music and artwork you own or have permission to distribute.
- If you want to keep the repository private, check the current GitHub Pages plan and repository eligibility first.
