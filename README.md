# MkDocs-tutorial

```
$ git config --global core.editor 'code --wait'
```

## Reference
- [MkDocs](https://www.mkdocs.org/)

## Installation

:information_source: Note

If you are using `Windows`, some of the above commands may not work out-of-the-box.

A quick solution may be to preface every Python command with `python -m` like this:
```
python -m pip install mkdocs
python -m mkdocs
```
For a more permanent solution, you may need to edit your `PATH` environment variable to include the `Scripts` directory of your Python installation. Recent versions of Python include a script to do this for you. Navigate to your Python installation directory (for example `C:\Python38\`), open the `Tools`, then `Scripts` folder, and run the `win_add2path.py` file by double clicking on it. Alternatively, you can download the script and run it (`python win_add2path.py`).

## Creating a new project
```
$ python -m mkdocs serve
INFO     -  Building documentation...
INFO     -  Cleaning site directory
INFO     -  Documentation built in 0.08 seconds
INFO     -  [23:34:57] Serving on http://127.0.0.1:8000/
INFO     -  [23:35:02] Browser connected: http://127.0.0.1:8000/
```

## Help
    $ python -m mkdocs -h
    Usage: __main__.py [OPTIONS] COMMAND [ARGS]...
    
      MkDocs - Project documentation with Markdown.
    
    Options:
      -V, --version  Show the version and exit.
      -q, --quiet    Silence warnings
      -v, --verbose  Enable verbose output
      -h, --help     Show this message and exit.
    
    Commands:
      build      Build the MkDocs documentation
      gh-deploy  Deploy your documentation to GitHub Pages
      new        Create a new MkDocs project
      serve      Run the builtin development server
