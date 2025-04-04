# langtail/docs

This is the source code for Langtail documentation. You can visit https://langtail.com/docs/ to read the docs.

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

### Screen casting

We're using screen studio for screen casts.

You can use the langtail.screenstudiopreset for our config. For export, use 1080p 30FPS MP4 in Web quality. Also keep the screen studio project files next to all MP4 in git.

### Image Compression

After taking a screenshot, we compress it using the following script using ImageMagick and optiPNG:

```bash
convert screenshot.jpeg -resize 1400x screenshot.png
optipng output.png
```
