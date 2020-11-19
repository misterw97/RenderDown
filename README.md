# RenderDown

Please refer to [upstream](https://github.com/jeffhung/RenderDown).

This version takes a data directory filled with yaml files, inject it in the template, and output matching markdowns.

## Usage

```sh
pip install -r requirements.txt
python renderdown.py template --outdir out --data ./data/
```

## Templates

Templates are rendered with [Mako][https://docs.makotemplates.org/en/latest/syntax.html]. A `doc` variable is added to the
namespace of all templates (see [API.md](API.md#renderdown-DocManager)
for a description of the functions on `doc`). For example, if
`mytemp.mako` is a template defined as follows:
