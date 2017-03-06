# Source Emoji

😃 Source Emoji is an emoji font project that began development in order to provide monochrome representative glyphs to the [Unicode Consortium](http://unicode.org/) for emoji candidates that have been accepted by the UTC (Unicode Technical Committee) but have not yet been fully ratified to become a part of the official standard.

The glyph artwork has been designed to harmonize with other Source fonts. The ultimate goal for this project is to grow it *slowly* over time to cover the full set of characters in Unicode that can take emoji presentation and eventually include colored SVG artwork for greater usability as emoji.

Currently the font can be considered as an alpha version. It features black & white artwork for supported emoji. There is no color artwork at the present.

## Characters currently supported

* Character support is generally inconsistent, but does contain glyphs for all Unicode 9 emoji.
* Most of the smiley characters are present.
* The glyphs for some characters are not adequately differentiated and may display as duplicates of other characters.
* Much of the artwork is still unfinished and can be considered provisional.
* Flag combinations will display as two-letter control pictures.
* Characters not in this font will display as a sad alien as a fallback.

## Building the fonts from source

### Requirements

To build the binary font files from source, you need to have installed the
[Adobe Font Development Kit for OpenType](http://www.adobe.com/devnet/opentype/afdko.html) (AFDKO). The AFDKO
tools are widely used for font development today, and are part of most font
editor applications.

### Building the font

The key to building OTF fonts is `makeotf`, which is part of the AFDKO toolset.
Information and usage instructions can be found by executing `makeotf -h`.

In this repository, all necessary files are in place for building the OTF font.
For example, build the binary OTF font like this:

```sh
$ makeotf -f SourceEmoji-BnW.ufo -r
```

## Getting involved

If you would like to contribute to this project, a template SVG file has been provided for creating SVG artwork to be incorporated into the UFO project. If you have comments or suggestions on how you would like to see this project develop, please leave feedback in the [Issues](https://github.com/adobe-fonts/source-emoji/issues) tracker for this project. Alternatively, you may send suggestions for changes to the Source Emoji font project maintainer, [Paul D. Hunt](mailto:opensourcefonts@adobe.com?subject=[GitHub] Source Emoji), for consideration.
