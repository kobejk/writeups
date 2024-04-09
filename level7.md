# Level 6 -> 7

**URL:** [OverTheWire Bandit Level 6 -> 7](https://overthewire.org/wargames/bandit/bandit7.html)

**Goal:** The password for the next level is stored somewhere on the server and has all of the following properties:
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size

**Solution:**
Use `find` to search across the server for the file meeting these criteria. To avoid permission denied errors cluttering the output, redirect errors to `/dev/null`:

    find / -user bandit7 -group bandit6 -size 33c 2>/dev/null

This will list files matching the criteria. Once located, use `cat` to read the password:

    cat /var/lib/dpkg/info/bandit7.password

**Password:** z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S