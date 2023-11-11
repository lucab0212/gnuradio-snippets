# gr-snippets
Tips and tricks for using GNU Radio with examples

## `param_file_picker`
Usage:
```
./param.py --file sine.wav
```
In GNU Radio it is not possible to change file source and  sink paths over variables or parameters.
This example implements a workaround: the source file set in the flowgraph (`.../CURRENT_FILE`) gets replaced by
the file you specify in `--file` through a python snippet that is executed before starting the flowgraph. 
