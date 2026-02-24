# everforest-factory 🏭
![License](https://img.shields.io/github/license/paulopacitti/everforest-factory?color=a7c080&style=flat-square)
![PyPI](https://img.shields.io/pypi/v/everforest-factory?color=e67e80&style=flat-square)

> _"Comfortable & Pleasant Color Scheme for Vim"_ - [sainnhe](https://github.com/sainnhe)

![example of everforest-factory](https://raw.githubusercontent.com/paulopacitti/everforest-factory/master/example.png)

- A simple `cli` to ~~convert~~ manufacture an [everforest](https://github.com/sainnhe/everforest) themed wallpaper.
- Three color palettes: *dark*, *light* and smooth *mix*.

## Requirements

- Python 3.13.1 or higher

## Installation

### From PyPI

```bash
pip install everforest-factory
```

### From source

```bash
git clone https://github.com/paulopacitti/everforest-factory.git
cd everforest-factory
pip install .
```

For development (editable mode):

```bash
pip install -e .
```

> **Note:** if `pip install` reports that the script is installed in a directory not on PATH (e.g. `/var/data/python/bin`), add it:
> ```bash
> export PATH="/var/data/python/bin:$PATH"
> ```
> Or run directly via `python -m factory`.

## Usage

```
everforest-factory [-h] [-p [{dark,light,mix}]] [-i IMAGES [IMAGES ...]]
```

### Options

| Flag | Description |
|------|-------------|
| `-h`, `--help` | Show help message and exit |
| `-p`, `--palette` | Choose palette: `dark` (default), `light`, or `mix` |
| `-i`, `--images` | Path(s) to the image(s) to process |

### Examples

**Convert a single image with the dark palette (default):**

```bash
everforest-factory -i wallpaper.png
```

**Use the light palette:**

```bash
everforest-factory -p light -i photo.jpg
```

**Process multiple images at once:**

```bash
everforest-factory -p mix -i image1.png image2.jpg image3.webp
```

**Use a glob pattern:**

```bash
everforest-factory -p dark -i ~/Pictures/*.png
```

**Run without installing (from the project directory):**

```bash
python -m factory -p dark -i wallpaper.png
```

### Output

Processed images are saved in the same directory as the originals with the `everforest_` prefix:

```
wallpaper.png → everforest_wallpaper.png
```

## Palettes

| Palette | Description |
|---------|-------------|
| `dark`  | Everforest Dark — deep green-tinted backgrounds with warm accents |
| `light` | Everforest Light — soft cream backgrounds with vivid accents |
| `mix`   | Extended blend of both dark and light palettes with intermediate tones |


## Contributors
Thanks for all the have been working with me to make this tool to craft beautiful wallpapers 🧡 
- [@H4ppy-04](https://github.com/H4ppy-04)
- [@Gabulhas](https://github.com/Gabulhas)
- [@hza2002](https://github.com/hza2002)
- [@jasonmishi](https://github.com/jasonmishi)
- [@perpetualCreations](https://github.com/perpetualCreations)
- [@Kuuhhl](https://github.com/Kuuhhl)
- [@marcelofern](https://github.com/marcelofern)

Also, I could not do this without the [ImageGoNord](https://github.com/Schroedinger-Hat/ImageGoNord-Web) project, go check them out!
