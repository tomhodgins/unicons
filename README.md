# Unicons

Unicons.css is a lightweight supplement or replacement for icon fonts like FontAwesome, as well as a semantic way to add unicode characters to your HTML markup.

It contains character codes for some of the hard-to-reach but useful characters buried deep within your font and giving us an easy way to select those using custom data attributes in HTML. This keeps your markup semantic and easy to edit, and lets you leverage many icons that may be installed on your target devices already without loading additional resources.

FontAwesome and other web-geared icon fonts are designed with icons for web applications, but the unicode standard which `unicons.css` supports includes general purpose pictograms that can also be useful in web applications as well as valuable mathematical, scientific, and international symbols that seem largely absent from websites today.

## How to install Unicons

`<link href="unicons.css" type="text/css" rel="stylesheet">`

## How to add Unicons into your HTML Markup

You can add Unicons to your HTML markup by applying the `data-unicon` HTML custom data attribute to any element, like the `<span>` element, by adding the name of the unicode character you want to insert as the attribute value. All names are written in lowercase letters with the spaces delimited by hyphens (-).

`<span data-unicon="black-heart-suit"></span>`

The above HTML code would insert the '&#x2665;' character.


## Supplying your own Font (recommended)

Right now unicons is simply a CSS file and a demo HTML character palette. Before using unicode characters in your project you need to be sure of two things: **1) you can anticipate which fonts these characters will display in**, and **2) the font this displays in supports the character you're trying to insert**. Unicons comes with no icons or font files of its own, so you may find varying support if you rely on the system fonts installed across different devices.

For a more bulletproof approach, supply your own font using `@fontface` in CSS. This way all visitors to your site will have the same support. You can select a font that supports the unicode characters you are looking for, and the [Deja Vu](http://www.fontsquirrel.com/foundry/DejaVu-Fonts) font project is a great starting place to find free fonts you can embed online with excellent unicode suppport.

- Check out the list of [Open-source Unicode typefaces](http://en.wikipedia.org/wiki/Open-source_Unicode_typefaces) to find other free embedding possibilities
- Create tailored versions of fonts for embedding online with [FontSquirrel's @fontface generator](http://www.fontsquirrel.com/tools/webfont-generator)
- [The @Font-Face Rule And Useful Web Font Tricks](The @Font-Face Rule And Useful Web Font Tricks) from Smashing Magazine

**TIP:** If you embed a custom font to use with `unicons.css` be sure to add a custom CSS style somewhere else in your project instructing unicons to use it. If you wanted to use a font named _'Custom-Font'_ you would add a snippet like:

    [data-unicon] { font-family: 'Custom-Font'; }


## Thanks

Big thanks to Dave Gandy and [Font Awesome project](https://github.com/FortAwesome/Font-Awesome) right here on Github for setting the bar for icon typography online, and for developing so many creative ideas about how to insert characters from a web font into CSS.

Another thanks out to [FontSquirrel](http://www.fontsquirrel.com) for making is easy to convert fonts to web formats, and lastly a shoutout to the [Deja Vu project](http://dejavu-fonts.org/wiki/Main_Page) for making one free fonts with excellent unicode glyph support!