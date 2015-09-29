general
=======

general.py Version 1.0.0

Functions for common tasks (e.g. opening files with exception handling built in). Works with either python 2.7+ or python 3.3+.

   USAGE: import general


FUNCTIONS:

```
convert_to_full(path)
```

Returns absolute path from a relative path.

```
mk_out_sub_directory(path)
```

Create directory (run after testing the existence of the
parent directory). Block only warns if output directory
already exists. Returns the boolean value True or False.

```
open_file(file_name)
```

Returns opened (for reading) file object or kills program and relays
error from running the open function as a log message. If error is of
unexpected type returns content of the error message but attempts
to keep runnning.

```
open_write_file(file_name)
```

Returns opened (for writing) file object or kills program and relays
error from running the open function as a message. If error is of
unexpected type returns content of the error message but attempts
to keep runnning.

```
parse_filename(file_name)
```

Returns path (with no trailing slash), basename and extension for filenames.

```
path_check(path)
```

Throw fatal error if path doesn't exist, otherwise return the boolean value True.

```
print_no_newline(to_print)
```

Print a statement without a new line in either python 2.7+ or python 3.3+