# dmenu inline prompt

This patch modifies dmenu so that, instead of displaying the prompt in front of the input, the prompt is shown as placeholder text inside the input field. When no text is typed, the placeholder appears; when you start typing, your input replaces it.

![dmenu with inline prompt](/img/header.png)

## Features

- Displays the prompt as placeholder text inside the input field when empty.
- Cursor (`|`) only appears when typing, keeping the field visually clean when empty.
- Build on latest version of dmenu (5.4)

## Installation

1. If you start off fresh, clone the dmenu repo from suckless.org

```bash
git clone https://git.suckless.org/dmenu
```

2. Clone this repo

```bash
git clone https://github.com/daanblom/dmenu-inlineprompt.git
```

3. Apply the patch (from your dmenu directory):

```bash
patch -p 1 < /path/to/inlinePompt.patch
```

4. Compile and install dmenu:

```bash
sudo make clean install
```

## Usage

No changes in usage. Run dmenu as usual:

## Notes

- Based on the base build of dmenu.
- build in header image at https://github.com/daanblom/suckless

## License

Follow the same license as dmenu (MIT/X11).
