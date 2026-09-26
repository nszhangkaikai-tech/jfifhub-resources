# JFIF conversion notes

JFIF is a JPEG interchange format commonly identified by `.jfif`, `.jfi`, or `.jif` file names. A browser conversion step can decode a supported image, draw it to a canvas, and export a JPEG blob.

## Integration checklist

1. Accept the three JFIF-family extensions in the file picker and drag-and-drop handler.
2. Keep conversion local when privacy matters: create an object URL, decode the image, draw it to a canvas, and export JPEG.
3. Make the output extension match the selected output (`.jpg` or `.jpeg`).
4. Expose a quality control and state its default clearly. JfifHub defaults to Highest (100%).
5. Revoke temporary object URLs after decoding or downloading.

The live implementation and user-facing behavior are at https://jfifhub.com/.
