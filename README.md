# RhythmNoteVerse

Vue + Web MIDI flash-card prototype for rhythm and note-reading practice.

## Run

Use a local server so `mapping.json` can be loaded:

```powershell
python -m http.server 5174
```

Then open `http://localhost:5174`.

## Assets

- The default City Pop background is saved at `assets/bg/city-pop-rhythm.png`.
- Cards are generated with inline SVG and HTML, so no card image folder is needed.
- Edit `mapping.json` only when you want to override card titles or explanations.
