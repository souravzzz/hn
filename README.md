hn
==

A CLI and Python library for [HNSearch's
API](http://www.hnsearch.com/api) that's easy-to-use.


Usage
-----

### Search

Basic search terms and querying. Allows for specifying number of results
with `n` flag (maximum is 100), and starting ordinal position of results
with the `s` flag.

```
hn search term
hn search term -n 100
hn search term -n 100 -s 100
```

### Date

The `d` flag allows for searchs filtered to a specific date (in
`YYYY-MM-DD` format).

```
hn -d 2012-03-16

hn search term -d 2012-01-01
```

### Sorting

By default, sorting will be descending.

```
hn techcrunch -S points

hn -d 2012-03-16 -S username asc
```

### Type

The `T` flag allows filtering by specific types of items (comment,
submission, etc).

```
hn zachwill -T comment
hn zachwill -T submission -S points
```
