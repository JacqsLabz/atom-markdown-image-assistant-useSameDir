# About

Please see [atom-markdown-image-assistant](https://atom.io/packages/markdown-image-assistant) for the full readme about what most of this package does. 99% of this package is the code from that package, so credit to [Tamas Nagy (tlnagy)](https://github.com/tlnagy) for his work in writing most of this code.

I've only added 2 very small things:

I probably coded this in an ineffiecent manner, but I've added a setting for using the same directory for the images as the markdown file. When it is checked/enabled, the asset folder setting is totally ignored/bypassed, so images get copied to whatever folder the markdown file is inside. This produces "!\[](/filename.jpg)" in the markdown file and the [atom markdown preview package](https://atom.io/packages/markdown-preview) doesn't seem to mind the extra / before the file name.

I also noticed that the [markdown preview package](https://atom.io/packages/markdown-preview) can't understand spaces in file names, and my image files have spaces in their file names. So, after the file is copied with the spaces in the file name intact, I've added a quick encodeURIComponent before that same file name is inserted into the editor. This only affects the file name not the asset path (I don't need the asset path, so I'm not bothering with it). 
