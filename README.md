# My CheatSheets

This is a personal project to collect all usable keyboard shortcuts for some applications, my goal is to create a printable pdf version of the collection.

It takes an html template file in jinja2 format, and generates the corresponding htmls, for later on, convert it to pdf.

In order to achieve this, it uses:
- https://symbl.cc/en/collections/arrow-symbols/ ( for especial symbol html entities )
- https://flowbite.com/docs/components/kbd/ ( nice lib for managing tailwindcss )
- https://github.com/fastily/jinja2html ( the main converter )
- https://tailwindcss.com/ ( for better tune in the design )

## Application List

 - kitty (https://sw.kovidgoyal.net/kitty/overview/)

## Generation

You need to install **jinja2html** via repository:
```
pip install jinja2html
```

or locally, downloading the source code and executing:
```
pip install .
```

after this, the executable will be located at ```~/.local/bin/jinja2html```

Then you can generate the file as:
```
cd src/kitty
jinja2html
```

Finally, you can:
- locate the the generated html on the "**out**" folder
- open it in chrome browser,
- and print to PDF, at 80% (so it can fit in one page).
