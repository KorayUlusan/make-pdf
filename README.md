# make-pdf

*CLI managment tool for scanned documents*

I like my pen and paper[1] and I like my computer. So my workflow consists some scanning and converting to pdf. This tools purpose is to make this fast and convenient.

And no, I don't like to scan to pdf.

[1]: This does not mean I don't like Latex. For me, they have different purposes. I am no Evan. Just watch [this](https://youtu.be/DsjGz_5m4Uk?t=2122) for 2:30 mins.

## Usage

```text
make-pdf - Koray's managment tool for scanned documents

Parameters:
  -h, --help        show this help message and exit

  <name>            creates a pdf called <name> on ~/Desktop
                    and then moves images to a folder called <name>. To disable
                    this behavior pass `-nw` to args

  ls                `ls ~/Scans`
  ll                `ls -lh ~/Scans`
  open              `open ~/Scans`

  unwrap <folder>   move <folder> contents to ~/Scans
  wrap <?folder>    moves files of ~/Scans to <?folder>
                    if no <?folder> is given. wraps to last unwrap.

Usage:
  make-pdf <name>
  make-pdf ll
  make-pdf open
  make-pdf unwrap <folder>
  make-pdf wrap <?folder>
```

Note: help text uses [fish style](https://fishshell.com/docs/current/cmds/prompt_pwd.html) path abbreviations

## Installation

MacOS:

- Install dependencies

  ```sh
  pip3 install img2pdf
  brew install imagemagick
  ```

- Add the executable to your `$PATH`.

You will probably want to change the default paths in the executable. You're welcome to do so.

## License

GNU Affero General Public License
