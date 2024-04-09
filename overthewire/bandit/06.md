# Level 5 -> 6

**URL:** [OverTheWire Bandit Level 5 -> 6](https://overthewire.org/wargames/bandit/bandit6.html)

**Goal:** The password for the next level is stored in a file somewhere under the `inhere` directory and has all of the following properties:
- human-readable
- 1033 bytes in size
- not executable

**Solution:**
Navigate to the `inhere` directory and use `find` to locate the file matching all specified criteria:

    cd inhere
    find . -type f -size 1033c ! -executable

Once you have located the file, use `cat` to read its contents and find the password:

    cat ./maybehere07/.file2

**Password:** P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU