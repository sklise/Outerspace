Outerspace
=========

A clean cut UI theme for Sublime Text 2 bastardised from the source code of [Soda] and [Centurion] and [Spacegray].

Outerspace was made out of a want for a bit higher contrast than other minimal themes. And also because I kept switching themes throughout the day.

No gradients, no 1px edges and not a thousand different icon sprites. Just color, shape and 14 [icons].

Installation
------------------------------------------------------------------------
### Package Control

Just install it and make sure to update your `Settings - User` file with:

    "theme": "Outerspace.sublime-theme"


### Manual

Clone it into your packages directory. These are OSX paths because I'm lazy like that. For Windows/Other just substitute your paths like a boss.

    cd ~/Library/Application Support/Sublime Text 2/Packages

    git clone git://github.com/allanhortle/Outerspace.git 'Theme - Outerspace'

Make sure you have the `Theme - Outerspace` at the end of the command so it is placed in the correct folder.
Unless of course you feel like experiencing the wrath of none icons.

Back to Sublime Text, press `super+,` to access your `Settings - User` and insert:

        "theme": "Outerspace.sublime-theme"

If it looks like crap make sure to restart Sublime before crying.

---

Custom Colors
-------------
I've re-written Outerspace to use [Grunt]. As a result you can now make your own
custom colored versions of the theme. If you haven't used grunt before, then you probably should learn. It's super amazing.

Because package control likes to cache and update installed packages I suggest cloning an extra copy of the Outerspace repo into your packages folder.
That way you'll still be informed of updates but you wont get your color constantly changed back to green.

I call mine `Theme - Outerspace_dev`. Im undecided as to whether or not this is the best option. But it works so this is how it will be for now.

_* Side note: if you call your folder something like `AAAOuterspaceRadColor` it might not take precedence over the original package. So if you do have two copies give it a name that is alphabetically lower than `Theme - Outerspace`._

### The actual instructions bit:

1. `cd` into the theme directory.
2. `npm install` To install the grunt dependancies.3.
3. Open up `Gruntfile.js` and look for `folderName:'Theme - Outerspace'`
4. Just make sure this matches what ever you have named the folder.
5. Next look for `config.hero = config.green;`
6. change the color to what ever radical choice you have in mind.You can use the predefined ones from Galea or go nuts with your own `[r,g,b]` combination.
7. Back to terminal and run `grunt`.
8. Close and reopen Sublime Text.
9. Ride an eagle into the sunset. You're all done.


---
## Galea
Outerspace now ships with it's own syntax highlighting. Galea is a simple theme designed to cut down on the use of color in conflicting locations. There are only five colors, each relating to a high level Textmate scope.

| Color         | Scope                |
| ------------- |----------------------|
| Yellow      	| Entity / Tag         |
| Red      		| Support / Keyword    |
| Orange 		| Storage    		   |
| Green         | String               |
| Blue          | Constant             |

Additionally each file's background is tinted to distinguish it's type. Front-end remains grey, backend is blue and data-files are green.

### Bugs
If you like the theme and  find some bugs please do let me know. I've been testing it only with my current pipeline so there are bound to be file types that miss out. Just bug it out and I'll do my best to fix them up.


[grunt]: http://gruntjs.com/ "It really is the business"
[soda]: https://github.com/buymeasoda/soda-theme/
[centurion]: https://github.com/allanhortle/Centurion
[spacegray]: https://github.com/kkga/spacegray
[icons]: http://www.glyphicons.com/
