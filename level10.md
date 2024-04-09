# Level 9 -> 10

**URL:** [OverTheWire Bandit Level 9 -> 10](https://overthewire.org/wargames/bandit/bandit10.html)

**Goal:** The password for the next level is stored in the file `data.txt` in one of the few human-readable strings, preceded by several '=' characters.

**Solution:**
Use `strings` to extract text strings from `data.txt`, then `grep` to filter lines with '=' characters:

    strings data.txt | grep '=='

This command isolates lines with human-readable strings preceded by '=' characters, helping to identify the password.

**Password:** G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
