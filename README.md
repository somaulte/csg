# CSG

`csg` is a **c**olor**s**cheme **g**enerator which takes a single colormask and outputs a tinted base16 colorscheme.  

### Dependencies

- `bash`

### Usage

```sh
Usage: csg {OPTION} color weight
Example: csg -c="~/documents/colors" -f '#12271c' 55 -g

	Options:
		-c='/path/to/colors'	Load colorscheme to compare against from external file.
					Color0-15 should be listed in this file as strings in bash syntax.
		-f			Set color0 to the input color.
		-g			Generate hilights from color0-7.
		-h, --help		Display this message.

	Arguments:
		color			A single color represented in hexadecimal format: '#FFFFFF'.
		weight			Value between 0 and 100, a higher number results in a
					color more closely resembling the input color.

	Environment variables:
		CSG_DEBUG		If set to 'true' or '1', enter debug mode.

```
