# Contributors

## Figma

The original Figma design file for the icons can be found here:

[Original Figma File](https://www.figma.com/design/QHSG0XBYimLFwMhYZ03hrS/Rljson?node-id=0-1&t=6b47KJI8G7f12Hqy-1)

Please feel free to create a PR of this repo containing additional helpful images.

## Export the files from Figma

Visit <https://www.figma.com/design/QHSG0XBYimLFwMhYZ03hrS/Rljson?node-id=0-1&t=6b47KJI8G7f12Hqy-1>

Press `Cmd+Shift+E`

Save the files to `~/tmp`

Convert the files to `webp`:

```bash
find ~/tmp/doc -type f -name "*.jpg" -exec sh -c 'cwebp "$1" -o "${1%.jpeg}.webp" && rm "$1"' _ {} \;
```

Copy over the files to this repo:

```bash
rm -rf doc/img
cp -r ~/tmp/doc/img doc/
```
