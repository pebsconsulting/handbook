# wp cache delete

Remove a value from the object cache.

Errors if the value can't be deleted.

### OPTIONS

&lt;key&gt;
: Cache key.

[&lt;group&gt;]
: Method for grouping data within the cache which allows the same key to be used across groups.
\---
default: default
\---

### EXAMPLES

    # Delete cache.
    $ wp cache delete my_key my_group
    Success: Object deleted.


