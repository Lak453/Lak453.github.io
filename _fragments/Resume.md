---
layout: fragment
title: Resume
tags: [Resume]
description: Resume
keywords: Resume
mermaid: false
sequence: false
flow: false
mathjax: false
mindmap: false
mindmap2: false
---

In VSCode, the default Markdown preview style is not very visually appealing. You can customize the style.

To do this, go to the VSCode settings, find Extensions > Markdown > Markdown: Styles, and then Add Item. You can add a local CSS file from the current working directory or a URL.

Issues encountered:

1. The local CSS file cannot be an absolute path outside the current working directory, otherwise, an error will occur.
2. The media type of the URL address must not be text/plain, otherwise, an error will occur: `Could not load 'markdown.styles'`. Reference: <https://github.com/microsoft/vscode/issues/148677>.
