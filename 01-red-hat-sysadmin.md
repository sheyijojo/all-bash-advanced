```yaml


sudo sed -i 's/enabled/disabled/gi' -l 500,2000 /home/bob/values.conf

```

The `sed` command you provided performs an in-place replacement within the file `/home/bob/data.txt`. Here's a breakdown of what it does:

### Command Explanation:
```bash
sed -i 's~#%$2jh//238720//31223~$2//23872031223~g' /home/bob/data.txt
```

1. **`sed`**: The stream editor command.
2. **`-i`**: This flag tells `sed` to edit the file in place.
3. **`s~...~...~g`**: The substitution command:
   - `s` indicates substitution.
   - `~` is the delimiter (used instead of the default `/` to avoid conflicts with the slashes in the pattern).
   - `#%$2jh//238720//31223`: The search pattern.
   - `$2//23872031223`: The replacement text.
   - `g`: Global flag, meaning all occurrences of the pattern in each line will be replaced.
4. **`/home/bob/data.txt`**: The file being modified.

### What It Does:
- Replaces all occurrences of `#%$2jh//238720//31223` with `$2//23872031223` in the file `/home/bob/data.txt`.

### Example:
#### Before:
```
#%$2jh//238720//31223
Another line
#%$2jh//238720//31223
```

#### After:
```
$2//23872031223
Another line
$2//23872031223
```



```yaml
egrep -rw '[A-Z][a-z]{2}' /etc/nsswitch.conf > /home/bob/filtered1

In /home/bob/textfile file there's a number that has 5 digits. Save the same in /home/bob/number file.:


You can use the redirection to save your command's output in a file i.e [your-command] > /home/bob/number:
egrep '[0-9]{5}' textfile > /home/bob/number






How many numbers in /home/bob/textfile begin with a number 2, save the count in /home/bob/count file.


You can use the redirection to save your command's output in a file i.e [your-command] > /home/bob/count
grep -c '^2' textfile > /home/bob/count




How many lines in /home/bob/testfile file begin with string Section, regardless of case.
Save the count in /home/bob/count_lines file.

grep -ic '^SECTION' testfile > /home/bob/count_lines


Find all lines in /home/bob/testfile file that contain string man, it must be an exact match.

For example the line like # before /usr/man. or NOCACHE keeps man should match but # given manpath. or For a manpath must not match.


Save the filtered lines in /home/bob/man_filtered file.


grep -w man testfile > /home/bob/man_filtered




Save last 500 lines of /home/bob/textfile file in /home/bob/last file.

tail -500  /home/bob/textfile > /home/bob/last

```

