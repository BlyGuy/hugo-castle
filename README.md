# Hugo Castle

A hugo theme for my personal blog/portfolio-site [https://marchoek.nl](https://marchoek.nl).

That site also serves as an example for the theme.

## Features

* Just HTML/CSS
* Doors
* (Kinda) *Mediaeval* Interior by default

## Installation

Many ways to do this but I recommend adding this as a git submodule for easier updating later on:

```sh
git submodule add --depth=1 https://github.com/BlyGuy/hugo-castle.git themes/hugo-castle
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
```

Now add `theme = 'hugo-castle'` to your `hugo.toml` in the root directory of your hugo site.

## Updating

If you chose to install the theme using the method above,
updating is as easy as typing this command while in your hugo-site.

```sh
git submodule update --remote --merge
```

## Configuration

To tweak existing assets in the theme copy these to your own site first and edit them there.
For example, if you wanna edit the main stylesheet of the theme, copy the file like so:

```sh
cp themes/marc_style/assets/css/main.css assets/css/main.css
# You can now edit assets/css/main.css however you please
```

I also recommend adding custom doors to your site,
(unless you want to have the doors look like the example-site, of course):

```sh
cp themes/marc_style/static/door1.png themes/marc_style/static/door2.png static
# You can now edit static/door1.png and static/door2.png, have fun :)
```
