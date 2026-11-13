# JavaScript Text to Speech

A browser application that reads entered text aloud using the Web Speech API.

## Features

- Speak text entered by the user.
- Pause, resume and stop playback.
- Choose from predefined voice options.
- Adjust speech speed using the interface controls.

## Built with

HTML, CSS and vanilla JavaScript. The application uses `SpeechSynthesisUtterance` and the browser's `speechSynthesis` interface; it does not train a speech model.

## Run locally

Clone the repository and open `index.html` in a browser with speech synthesis support. No package installation or build step is required.

You can also serve the directory locally:

```sh
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Code guide

- `index.html`: application interface.
- `style.css`: styling.
- `index.js`: speech playback, voice selection and speed controls.
- `assets/`: interface assets.

## Compatibility notes

Available voices depend on the browser and operating system. The current implementation selects voices by array index, so some predefined options may be unavailable or differ between devices. Voice loading and playback behavior should be checked in the intended browser.

## Author

[Hassan Robert](https://github.com/HassanR500) · [LinkedIn](https://www.linkedin.com/in/hassan-robert/)
