# ytsearch

A handle little utility for returning the top youtube result for a given query.

Note that this implementation is designed for Python 2. It is based off of a
similar implementation [here](https://www.codeproject.com/Articles/873060/Python-Search-Youtube-for-Video)
but modified to work for Python 2.7 and using from the command line.

This implementation was designed mainly for the use of retriving Youtube URLs
for music videos. As such, by default it searches for the **official video**
version of the result. This behaviour can be overriden with either the `-n`
flag passed on the command line, or by setting the optional keyword argument
`official_video` to `False`.

## Example Usage

Can be used either from the command line or directly imported into another
python project.

### Command line

    $ ./ytsearch thrift shop
    https://www.youtube.com/watch?v=QK8mJJJvaes
    $ ./ytsearch -n dogs barking
    http://www.youtube.com/watch?v=DXUAyRRkI6k

### Python interpreter

    >>> import ytsearch
    >>> ytsearch.geturl("thrift shop")
    https://www.youtube.com/watch?v=QK8mJJJvaes
    >>> ytsearch.geturl("dogs barking", official_video=False)
    http://www.youtube.com/watch?v=DXUAyRRkI6k

