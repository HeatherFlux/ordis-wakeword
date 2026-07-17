# Ordis wake word (microWakeWord)

Custom "Ordis" wake word for ESPHome `micro_wake_word` (v2), trained locally with
[microWakeWord](https://github.com/kahrendt/microWakeWord) on an RTX 4070.

- `ordis.tflite` — quantized streaming model (62 KB)
- `ordis.json` — ESPHome v2 manifest (`probability_cutoff` 0.97)

## Use in ESPHome
```yaml
micro_wake_word:
  models:
    - model: github://HeatherFlux/ordis-wakeword/ordis.json@main
```
Personal/home use. Trained on synthetic TTS audio.
