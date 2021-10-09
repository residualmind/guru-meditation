# Guru Meditation

*An attempt to re-create the iconic Guru Meditation error messages of AMIGA computers for the web.*

## Why? And why do I need this?

No reason, really. I have been watching a lot of retro computing content lately and felt like I had
to make something that tickles my nostalgia.

There is absolutely no need for this. Maybe if you're running an AMIGA website and want to display
nice error messages, you might actually have a use for this. I simply made it because I wanted to.


## Usage

### Import the class from the module

    import Guru from "./gurumeditation.js"

### Tell the Guru to meditate

The module exports one default class which has one static method called `meditate`. It takes one
(string) argument - the message to be displayed.

    Guru.meditate("All is good, nothing to worry about\nGuru Meditation #00001234.00005678");

The message can be closed by clicking on it.

There can only be one Guru Meditation at a time - if one is already being displayed when `meditate`
is called, the old message is replaced with the new one.

### Example

An example file is included. To see Guru Meditation in action, copy`example.html` and
`gurumeditation.js` next to each other onto a webserver and open the html in a browser.

## Notes

This is the very first attempt of creating the effect and not more than a sketch. What happens is
that a `HTMLDivElement` is created and prepended before the first child of the `document`. This has
worked for me on the DOM-Trees and JS codebases I tried it out - but it may horribly fail in other
cases - ***help me improve this if you want to***!

Also, if you have better ideas about how to package something as tiny as this, let me know.

## License

CC0 1.0 / ♡ Copyheart

## Inspiration
* [AMIGA Computers](https://en.wikipedia.org/wiki/Amiga)
* My childhood in [the 80s](https://en.wikipedia.org/wiki/1980s)
