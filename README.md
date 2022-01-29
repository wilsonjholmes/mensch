# mensch
Mensch is a [Zola](https://github.com/getzola/zola) theme roughly based on [Wolfgang's notthebe.ee site](https://notthebe.ee/) using gruvbox and the Inter font (a particular but favorite combo of mine :smile:).

![Hyde screenshot](https://f.cloud.github.com/assets/98681/1831228/42af6c6a-7384-11e3-98fb-e0b923ee0468.png)


## Contents

- [Installation](#installation)
- [Options](#options)
  - [Sidebar menu](#sidebar-menu)
  - [Sticky sidebar content](#sticky-sidebar-content)
  - [Themes](#themes)
  - [Reverse layout](#reverse-layout)

## Installation
First download this theme to your `themes` directory:

```bash
cd themes
git clone https://github.com/wilsonjholmes/mensch.git
```
and then enable it in your `config.toml`:

```toml
theme = "mensch"
```

## Options

### Sidebar menu
Set a field in `extra` with a key of `mensch_links`:
```toml
[extra]
mensch_links = [
    {url = "https://google.com", name = "Google.com"},
    {url = "https://google.fr", name = "Google.fr"},
]
```
Each link needs to have a `url` and a `name`.

### Sticky sidebar content
By default Mensch ships with a sidebar that affixes it's content to the bottom of the sidebar. You can optionally disable this by setting `mensch_sticky` to false in your `config.toml`.

#TODO
### Themes
Mensch ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

![Hyde in red](https://f.cloud.github.com/assets/98681/1831229/42b0b354-7384-11e3-8462-31b8df193fe5.png)

There are eight themes available at this time.

![Hyde theme classes](https://f.cloud.github.com/assets/98681/1817044/e5b0ec06-6f68-11e3-83d7-acd1942797a1.png)

To use a theme, set the `mensch_theme` field in `config.toml` to any of the themes name:

```toml
[extra]
mensch_theme = "theme-base-08"
```
#TODO
To create your own theme, look to the Themes section of [included CSS file](https://github.com/poole/hyde/blob/master/public/css/hyde.css). Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.

### Reverse layout

![Hyde with reverse layout](https://f.cloud.github.com/assets/98681/1831230/42b0d3ac-7384-11e3-8d54-2065afd03f9e.png)

Mensch's page orientation can be reversed by setting `mensch_reverse` to `true` in the `config.toml`.
