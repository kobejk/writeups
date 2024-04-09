# Level 3 -> 4

**URL:** [OverTheWire Bandit Level 3 -> 4](https://overthewire.org/wargames/bandit/bandit4.html)

**Goal:** Find the password in a hidden file within the `inhere` directory.

**Solution:**
Navigate to the `inhere` directory and use the `ls` command with the `-a` option to display all files, including hidden ones. Then, use `cat` to read the hidden file:

    cd inhere/
    ls -a
    cat .hidden

**Password:** 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe