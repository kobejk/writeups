# Level 8 -> 9

**URL:** [OverTheWire Bandit Level 8 -> 9](https://overthewire.org/wargames/bandit/bandit9.html)

**Goal:** The password for the next level is stored in the file `data.txt` and is the only line of text that occurs only once.

**Solution:**
Sort `data.txt` and use `uniq` to filter out the unique line. The `-u` option with `uniq` shows only unique lines:

    sort data.txt | uniq -u

This will display the line that occurs exactly once in `data.txt`.

**Password:** EN632PlfYiZbn3PhVK3XOGSlNInNE00t
