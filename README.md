
# Known problem:

## Does not support SVG

### Converting SVG's

`rsvg-convert -a -w 200 -h 200 rect.svg > rect-rsvg.png`

```
for file in *.svg; do
    filename=$(basename "$file")
    rsvg-convert -a -w 1000 -h 1000 "$file" > "${filename%.svg}.png"
done
```


Install imagemagick (sometimes this does not center)

`magick -background none -density 1000 -size 1000x dancers_trinity.svg dancers_trinity.png`




## Page Not Found

Probably it's the result of clone or pull without recursive.