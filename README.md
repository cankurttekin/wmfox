# A minimalist userChrome.css

This particular config works best with a minimalist WM like sway/i3, dwm, xmonad or
awesome.
This fork:
Moves tabs and url bar bottom. I prefer the main content to be at 
top of screen for more distraction free, cleaner look and ergonomic setup.

It also adds numbering on tabs so you can either use Alt+number or if you use 
vimium plugins number+g0 for switching to the tab you wish to go 
without guessing, cycling in ctrl+tab or even worse using mouse.

## How to use

Enable user chrome:

1) in `about:config` set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`

Enable compact mode:

1) in `about:config` set `browser.compactmode.show` to `true`
2) in the customize toolbar menu set `density` to `compact`

Via the customize toolbar menu remove firefox view (the top-left corner icon)

Copy `userChrome.css` to the `chrome` directory in your firefox profile. If
there is no such directory create it.

If you're unsure what the path to your profile's directory is, you can find out
by going to `about:profiles`.

Then either install the DejaVu Sans Mono font, or change the relevant line of
`userChrome.css` (search for 'DejaVu Sans Mono') to some other font that you have
installed. This affects the urlbar font.

Color of text in a tab is determined by its container. If a tab has no
container, fallback colors are used. You can change the basic colorscheme by
adjusting values of variables defined at the top of `userChrome.css`.

## Screenshots

![](./screenshots/screenshot.png)


## Common issues

### black stripe under tab bar

Increase the value of the `--tab-min-height` variable in `userChrome.css`.

### I want to disable favicons

Search for 'disable favicons' and uncomment the relevant line.

## Credit

[Dook97's firefox-qutebrowser-userchrome](https://github.com/Dook97/firefox-qutebrowser-userchrome)

[aadilayub's firefox-i3wm-theme](https://github.com/aadilayub/firefox-i3wm-theme)
