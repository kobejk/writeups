# Level 4 -> 5

**URL:** [OverTheWire Bandit Level 4 -> 5](https://overthewire.org/wargames/bandit/bandit5.html)

**Goal:** Identify the human-readable file among several in the `inhere` directory.

**Solution:**
First, navigate to the `inhere` directory. Then, use the `file` command to check the types of files starting with `-file0` to find the human-readable one:

    cd inhere/
    file ./-file0*

The output will reveal which file is ASCII text or similar. Read the content of that file using `cat`:

    cat ./-file07

**Password:** lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR