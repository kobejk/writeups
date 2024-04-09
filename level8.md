# Level 7 -> 8

**URL:** [OverTheWire Bandit Level 7 -> 8](https://overthewire.org/wargames/bandit/bandit8.html)

**Goal:** The password for the next level is stored in the file `data.txt` next to the word "millionth".

**Solution:**
Use `grep` to search `data.txt` for the line containing the word "millionth":

    grep 'millionth' data.txt

This command filters out the specific line with the password next to "millionth".

**Password:** TESKZC0XvTetK0S9xNwm25STk5iWrBvP
