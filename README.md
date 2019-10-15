# Matrix Converters

This package bundles functions which read and write various matrix file formats using nothing but the Scientific Python
stack (NumPy and Pandas). The idea is to allow closed-source software (e.g. Emme, VISUM, Cube, etc.) to "talk" to each
other through matrices.

Each format comes with a reader and writer, which converts to and from NumPy arrays or Pandas DataFrames. Pandas Series
with 2-level MultiIndex are also supported.

This was originally written by Peter Kucirek for Python 2.7 (or so). Upgraded to Python 3.6 by Andrew Rohne.

## Currently Supported Matrix Formats

I hope this list to grow over time with other formats.

- Emme 'internal' matrices (inside the Emmebank)
- Emme 'official binary' matrices
- FORTRAN-friendly BIN files (to work with Bill Davidson's code)


## Installation Instructions

1. Download the and unzip source from GitHub (click the download link at the top-right)
2. Open a command window in your unzipped directory (e.g. if you unzipped the source to "C:\matrix_converters", start
a cmd.exe in that folder
3. `python setup.py install`

Make sure that you've registered Python to you PATH environmental variable. Otherwise, you can launch pip from
<Anaconda>/Scripts/pip.exe.

## Usage

```
import matrix_converters as mc

matrix = mc.from_emx(*filepath\\filename.emx*)
```


## License

(c) WSP | Parsons Brinckerhoff
