# About

Please see [atom-markdown-image-assistant](https://atom.io/packages/markdown-image-assistant) for the full readme about what most of this package does. 99% of this package is the code from that package, so credit to [Tamas Nagy (tlnagy)](https://github.com/tlnagy) and everyone else who contributed and their work in writing most of this code.

I've only added 2 very small things:

I've added a setting for using the same directory as the markdown file for the images. When it is checked/enabled, the asset folder setting is totally ignored/bypassed.

I also noticed that the [markdown preview package](https://atom.io/packages/markdown-preview) can't understand spaces/special characters in file names, and my image files have weird spaces in their file names. So, after the image file is copied with the spaces in the file name intact, I've added a quick encodeURIComponent before that same file name is inserted into the editor. This only affects the file name not the asset path (I don't need an asset path, so I didn't mess with it).
