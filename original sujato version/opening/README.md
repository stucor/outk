# README.md

PDF:

- install tex-live-full (or other complete LaTeX)
- install these fonts on your system: Alegreya, Alegreya Sans, Symbola
- run `lualatex opening.tex` (twice to update ToC)

EPUB:

- `pandoc opening.tex -o opening.epub`
Note that the resulting EPUB has almost no styles, which especially impacts the aphorisms. I have added .center and .itshape classes. 

```
  .center{
    text-align: center
}
.itshape{
  font-style: italic
}

```

But if the file is regenerated, these will have to be added again. If more extensive styling needs to be done, add a second style sheet and keep it separately.