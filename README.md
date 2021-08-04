# Music Examples for Music Suite
This repo contains example projects that I've put together while exploring the 
[MusicSuite](https://github.com/music-suite/music-suite) application

You can also use this structure as a template for your own projects.


## How to run examples
You will need lilypond and a midiplayer installed on your system (e.g. timidity).

Replace `<input>` and `<output>` with the path to the haskell file and the output file.
### Lilypond

```
stack exec runhaskell -- <input>.hs -f ly -o <output>
lilypond -dbackend=eps -dno-gs-load-fonts -dinclude-eps-fonts -dresolution=400 --png <output>
```

### MIDI

```
stack exec runhaskell -- <input>.hs -f mid -o <output>
```

### Other Options
```
-f xml
-f ly+mid
```
