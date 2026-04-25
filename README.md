# RhythmNoteVerse

RhythmNoteVerse is a browser-based music theory and note-reading card app built with Vue and Web MIDI.
It presents pitch cards, rhythm cards, clefs, rests, accidentals, and basic theory concepts in a flash-card style interface designed for beginner-friendly learning.

## Demo

Live demo:
`https://piano.a-long-vacation.com/`

## Features

- Web MIDI input support for triggering pitch cards from a connected keyboard
- Flash-card interaction with front and back card views
- SVG-rendered notation instead of static card images
- Theory card library for note values, rests, clefs, and accidentals
- Random card draw and quick card selection
- Contact form for user feedback
- GitHub shortcut inside the app UI

## Tech Stack

- Vue 3 via CDN
- Plain HTML, CSS, and JavaScript
- Web MIDI API
- FormSubmit for contact form delivery

## Project Structure

```text
RhythmNoteVerse/
|-- index.html
|-- style.css
|-- mapping.json
|-- README.md
|-- LICENSE
`-- assets/
    `-- bg/
        `-- city-pop-rhythm.png
```

## Getting Started

1. Clone the repository:

```powershell
git clone https://github.com/dockvader/RhythmNoteVerse.git
cd RhythmNoteVerse
```

2. Start a local static server:

```powershell
python -m http.server 5174
```

3. Open the app in your browser:

```text
http://localhost:5174
```

## Usage

- Connect a MIDI keyboard and press keys to open pitch cards.
- Use the quick selector to browse theory cards manually.
- Click a card to flip between the front and explanation side.
- Use the contact section to submit feedback from the website.

## Configuration

`mapping.json` is used to override default card content such as titles, reading tips, counting notes, and memory hints.

Example:

```json
{
  "cards": [
    {
      "id": "note-60",
      "title": "C4 / Do",
      "reading": "C4 is middle C on the treble staff ledger line below.",
      "counting": "Pitch does not determine duration; combine it with note value cards.",
      "memory": "Middle C connects treble and bass staff reading."
    }
  ]
}
```

## Contact Form

The built-in contact form uses FormSubmit.
The current form action is configured in `index.html` and sends submissions through the FormSubmit endpoint associated with this project.

## Deployment

Because the app is a static site, it can be deployed easily to platforms such as:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages

## License

This project is licensed under the MIT License.
See [LICENSE](./LICENSE) for details.
