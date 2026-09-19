# Media folder convention

Drop images/GIFs here, named after the exercise `id` from `src/data/exercises.json`:

```
public/media/<exercise-id>.jpg    (or .png)
public/media/<exercise-id>.gif
```

Example: for the exercise with `id: "front-split-active"`, add:

```
public/media/front-split-active.jpg
public/media/front-split-active.gif
```

The app checks for a file at that path automatically — you don't need to edit
`exercises.json`'s `media` field by hand for files placed this way. If both a
`.gif` and a `.jpg`/`.png` exist for the same id, the GIF is preferred in the
player and the still image is used in the library browser.

If no matching file exists, the app shows a placeholder icon with the
exercise's text cues instead of a broken image.
