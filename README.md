# cv

How to put together a richly formatted document (in this case, a resume) using only Markdown + CSS!

PDF export is done via the VS Code extension ["Markdown PDF" by yzane](https://github.com/yzane/vscode-markdown-pdf).

## Why?

This approach lets you mix-and-match the speed and convenience of Markdown with the customisation of CSS. Whether it's worth it (versus straight Markdown, or regular HTML + CSS) probably depends on your use case and the amount of styling you have to do.

If your text is to be very richly formatted, might be better to use straight HTML + CSS (or Latex or Word). If your text frequently needs to be updated or shuffled around, and you just need a few tweaks above what Markdown can provide, this might work well for you!

Note: Markdown PDF exports to HTML in addition to PDF, so you can actually just ditch the Markdown altogether at a later date if you wish. See the [export](export) directory for an example.

## Styling

Tailwind-mimicking classes are defined in `markdown-pdf.css` as needed.

You could directly use Tailwind CSS instead, for example via the [standalone binary](https://github.com/tailwindlabs/tailwindcss/releases), if re-defining CSS classes seems like too much work for you.

Define a script like:

```bash
#!/bin/sh
./tailwindcss -i input.css -o output.css --watch
```

## Icons

The GitHub icon is from GitHub.

Credit to [Font Awesome](https://fontawesome.com) for the rest of the icons (Markdown PDF doesn't support comments inside SVGs):

```Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.```
