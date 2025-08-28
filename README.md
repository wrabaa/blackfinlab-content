# blackfinlab-content
Tutorial audio + metadata for the BlackFinLab app.   This repository hosts JSON manifests and media references (episodes, durations, artwork, stream URLs).   Used by the app to dynamically fetch new tutorials without needing an App Store update.
# BlackFinLab Content

This repository hosts **tutorial audio and metadata** for the **BlackFinLab** app.  
The app fetches this repo dynamically, so new tutorials can appear instantly without needing an App Store update.

---

## Structure
- `episodes.json` → master manifest file with episode metadata (title, duration, audio URL, artwork).
- `/audio/` → folder for tutorial audio files (optional, or linked from external CDN).
- `/artwork/` → optional artwork icons/images.

---

## Episode Manifest Example
```json
{
  "version": 1,
  "episodes": [
    {
      "id": "tut-0001",
      "title": "Nitrox Basics: PPO₂ & MOD",
      "duration_sec": 312,
      "audio_url": "https://example.com/audio/tut-0001.mp3",
      "pub_date": "2025-08-28",
      "artwork": "atom"
    }
  ]
}
