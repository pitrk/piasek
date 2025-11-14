# Mszalik na Uroczystość Niepokalanego Poczęcia Najświętszej Maryi Panny

Wymagania

```
lilypond
# np. brew install lilypond
```

Budowanie

```
lualatex --shell-escape mszalik.tex
```

Booklet

```
lualatex booklet.tex
```

Booklet w odcieniach szarości

```
gs \
  -sOutputFile=booklet-gray.pdf \
  -sDEVICE=pdfwrite \
  -sColorConversionStrategy=Gray \
  -dProcessColorModel=/DeviceGray \
  -dCompatibilityLevel=1.4 \
  -dNOPAUSE -dBATCH \
  booklet.pdf
```
