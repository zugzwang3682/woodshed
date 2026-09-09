# Woodshed

A fretboard and pattern engine for practising improvisation over modal vamps.
One self-contained HTML file — no build, no server, no dependencies.

## Launch

```
open ~/code/woodshed/woodshed.html
```

That opens it in your default browser. Bookmark the resulting `file://` URL
and it's a one-click launch from then on.

Everything runs locally: the theory engine, the pattern generator, the tab
importer, the beat detection, and playback. The only network request is the
Google Fonts stylesheet; offline it falls back to Georgia and the system
sans/mono and stays fully usable.

## Backing tracks

Drop an MP3 into the Backing track panel. It is decoded and analysed in the
page — spectral-flux onset detection, autocorrelation for tempo, a comb
search for phase — and the drill is then clocked off the audio itself, so it
cannot drift away from the record. Nothing is uploaded anywhere. Results are
cached per file, so a track is analysed once.
