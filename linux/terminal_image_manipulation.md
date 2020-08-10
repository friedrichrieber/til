# Image Manipulation in the Terminal with ImageMagick

## General 

These Examples will use [ImageMagick](https://imagemagick.org/) to manipulate iamges (e.g scaling, flipping). For more examples check the Source!


## Examples

### Convert Examples

Flipping an image 
```
convert test.jpg  -flip  flip.jpg
```

Mirroring an image 
```
convert koala.gif  -flop  flop.gif
```

### Mogrify Examples
(```mogrify``` is for replacing in place)


Scale the Image 25% down 
```
mogrify -scale 25% test.jpg
```

## Sources 

- [Example Website](http://www.imagemagick.org/Usage/basics/#mogrify)
- [ImageMagick Website](https://imagemagick.org/)
- [Reddit Post](https://www.reddit.com/r/commandline/comments/i6zhs8/common_imagemagick_examples/)
