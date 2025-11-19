# Level 9 --> 10

## 🎯Task 
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## ✅Solution 1

1. `strings data.txt | grep "====="`
   - `strings` finds human readable strings and prints them. This command is necessary as this file has a lot of non-printable characters
   - `grep` for `=====` among the readable strings and highlights them
3. Password - FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## ✅Solution 2

1. `vim data.txt`
   - opens the file data.txt
2. `/=====`
   - Type the above in command mode and you will be navigated to the occurrence of `=====`. Use n and N next and previous occurrences respectively
3. Password - FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
