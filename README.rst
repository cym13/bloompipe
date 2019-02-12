=========
Bloompipe
=========

What's this?
============

I felt the need to have a way to remove duplicates without loosing the
original order of input. Having some duplicate left was not an issue but it
was important for me to remove most of them.

(In case you're wondering I'm merging password dictionaries to crack hashes.)

So bloom filters are the exact data structure I need, and python-bloomfilter
is nice but somehow not easily available through pip or pacman or aur so I
just took the code and put it in one file with a 5-liner at the end to
produce bloompipe. Talk about lazy.

Anyway it does the job, pipe anything in, it outputs unique values. I used a
scalable bloom filter too so don't worry about dumping millions of lines,
it'll manage.

Original project
================

As explained 99% of the project is `python-bloomfilter
<https://github.com/jaybaird/python-bloomfilter>`_ so kudos to them. Really.

Dependencies
============

Check requirements.txt.

License
=======

I use the same MIT License as the original python-bloomfilter project by
design. Please be nice to them, that's good work there.
