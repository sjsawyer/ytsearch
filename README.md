# ytsearch

A handle little utility for returning the top youtube result for a given query.

Note that this implementation is designed for Python 2. It is based off of a
similar implementation [here](https://www.codeproject.com/Articles/873060/Python-Search-Youtube-for-Video)
but modified to work for Python 2.7 and using from the command line.


## Example Usage

Can be used either from the command line or directly imported into another
python project.

### Command line

    $ ./ytsearch thrift shop
    https://www.youtube.com/watch?v=QK8mJJJvaes

### Python interpreter

    >>> import ytsearch
    >>> ytsearch.geturl("thrift shop")
    https://www.youtube.com/watch?v=QK8mJJJvaes

