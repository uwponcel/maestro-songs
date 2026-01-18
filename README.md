# Maestro Community Songs

Community-contributed songs for the [Maestro](https://github.com/uwponcel/Maestro) Blish HUD module.

## Structure

- `manifest.json` - Index of all available songs with metadata
- `songs/` - Individual song files named by their UUID

## Contributing

1. Fork this repository
2. Add your song file to `songs/` with a new UUID
3. Update `manifest.json` with the song metadata
4. Submit a pull request

## Song Format

```json
{
  "name": "Song Name",
  "artist": "Original Artist",
  "transcriber": "YourUsername",
  "instrument": "Harp|Piano|Lute|Bass",
  "notes": ["C:500", "D:250", "E+:125"],
  "skipOctaveReset": false
}
```

### Note Format
- Note name: `C`, `D`, `E`, `F`, `G`, `A`, `B`
- Sharps: Add `#` (e.g., `C#`, `F#`)
- Octave up: Add `+` (e.g., `C+`, `D#+`)
- Duration in milliseconds after colon (e.g., `:500` = 500ms)
