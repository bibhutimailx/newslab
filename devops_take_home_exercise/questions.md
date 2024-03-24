# Questions

1. Diagram/explain the current architecture you're responsible for, and point out
where it's not scalable or fault-tolerant.

2. What are some examples of how you might scale a _read-heavy_ application? Why?

3. What are some examples of how you might scale a _write-heavy_ application? Why?

4. How do the following components get deployed in your current work environment,
from brain to production?
    a. Application code
    b. Configuration
    c. Infrastructure

5. In your opinion, what is the purpose of a post-mortem meeting?

6. How do you handle (and feel about) making changes (code/schema/network/etc.) in
your current environment? How do you know the changes you made did not break
anything?

7. Let's say you have a directory that contains other directories, that contain
Lucene/Solr indexes, that have these characteristics:

```bash
$ du -sh /search/data/
83G   /search/data/
$ find . -type d | wc -l
92
$ find . -type f | wc -l
35326
```
    a. What are 5 methods to copy this entire directory structure from one server to
another?
    b. What are any methods to speed up this transfer?
    c. How can you measure the resource usage of any of these different methods of
transfer? Do you expect any of them to use more CPU, more disk I/O, or more
memory?
