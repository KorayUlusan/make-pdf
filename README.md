# make-pdf

I like my pen and paper* and I like my computer. So my workflow consists some scanning and converting to pdf. This tools purpose is to make this fast and convenient. 

*: This does not mean I don't like latex. For me, they have different purposes. I am no Evan. Just watch [this](https://youtu.be/DsjGz_5m4Uk?t=2122) for 2:30 mins.

## Installation

Add the executable to your `$PATH`.

You will probably want to change the default paths in the file. You're welcome to do so.

## Usage

```text
make-pdf - create pdf from images

Parameters:
  -h, --help        show this help message and exit

  <name>            creates a pdf called <name> on ~/Desktop
                    and then moves images to a folder called <name>. To disable
                    this behaviour pass `-nw` to args

  ls                `ls ~/D/Scans`
  ll                `ls -lh ~/D/Scans`
  open              `open ~/D/Scans`

  unwrap <folder>   move <folder> contents to ~/D/Scans
  wrap <?folder>    moves files of ~/D/Scans to <?folder>
                    if no <?folder> is given. wraps to last unwrap.

Usage:
  make-pdf <name>
  make-pdf ll
  make-pdf open
  make-pdf unwrap <folder>
  make-pdf wrap <?folder>
```

Note: help text uses [fish style](https://fishshell.com/docs/current/cmds/prompt_pwd.html) path abbreviations

## License

to be determined

