# Recipe box

Personal recipe collection website

Powered by [Hugo](https://gohugo.io/) & [gochowdown](https://themes.gohugo.io/themes/gochowdown/) theme.

## Adding a new recipe

Use hugo template included with gochowdown to create a new recipe:

```bash
hugo new --kind recipe-bundle recipes/name-of-your-new-recipe
```


### Images

To remove EXIF data from images, you can use [ExifTool](https://exiftool.org/):

```bash
exiftool -all= -overwrite_original_in_place path/to/image
```

To easily resize images on the command line, install [ImageMagick](https://imagemagick.org/).
On OSX with homebrew installed, the easiest thing to do is:

```bash
brew install imagemagick
```

Once ImageMagick is installed, you can use mogrify to resize (among many other supported features, including converting format or applying filters):

```sh
mogrify -resize 1000x path/to/image
```
