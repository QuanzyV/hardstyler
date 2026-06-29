# Kick samples

These are the kick sounds that show up in the **Kick Sound** dropdown in HARDSTYLER.

## Add your own kick

1. **Drop your kick file in this folder** (`kicks/`). Use a short one-shot — `.wav` is safest; `.mp3`/`.ogg`/`.m4a` also work. Mono or stereo, any sample rate.
2. **Register it** by adding a line to [`kicks.json`](kicks.json):

   ```json
   [
     { "name": "Classic",     "file": "classic.wav" },
     { "name": "Raw / Hard",  "file": "raw.wav" },
     { "name": "My Kick",     "file": "my-kick.wav" }
   ]
   ```

   - `name` is what shows in the dropdown.
   - `file` is the exact filename you dropped here (case-sensitive).
3. Commit + push (or just reload if you're testing locally over a server). The new kick appears in the dropdown automatically.

## Notes

- Keep kicks short (roughly 0.1–0.6 s). Longer samples get retriggered on every beat and will smear.
- The **Synth (built-in)** option in the dropdown is generated live in the browser and isn't a file — it's always available, even offline.
- Sample kicks load over the network, so they work on the live site (or any local web server). If you open `index.html` straight from disk with `file://`, browsers block loading these files — use **Synth (built-in)** or the **Custom file…** picker there instead.
