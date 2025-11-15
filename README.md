---

# 🐚 OverTheWire – Bandit Walkthrough

A complete walkthrough documenting all levels solved, including commands, explanations, SSH login steps, and passwords.

---

# 🔐 **How to SSH Into Each Level**

Bandit requires you to SSH into a new account for each level.

### ✅ **General SSH Format**

```
ssh bandit<level>@bandit.labs.overthewire.org -p 2220
```

Example for level 5:

```
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

Enter the password you got from the previous level.

---

# **🔹 BEFORE LEVEL 0 — Starting Bandit**

The very first connection (Level 0 login):

### **SSH into Level 0**

```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

### **Password for Level 0:**

```
bandit0
```

---

# **🔹 Level 0 → 1**

### **How to SSH into this level**

```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists files in the directory
* `cat readme` reads the file containing the password

### **Password Found:**

**boJ9jbbUNNfktd78OOpsqOltutMc3MY1**

---

# **🔹 Level 1 → 2**

### **SSH into Level 1**

```
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists files
* `cat ./-` reads a file that starts with `-`

### **Password Found:**

**CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9**

---

# **🔹 Level 2 → 3**

### **SSH into Level 2**

```
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists files
* `cat "spaces in this filename"` reads the file with spaces

### **Password Found:**

**UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK**

---

# **🔹 Level 3 → 4**

### **SSH into Level 3**

```
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists files
* `cd inhere` moves into the folder
* `ls -a` shows hidden files
* `cat .hidden` reads the hidden file

### **Password Found:**

**pIwrPrtPN36QITSp3EQaw936yaFoFgAB**

---

# **🔹 Level 4 → 5**

### **SSH into Level 4**

```
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists files
* `file ./*` checks file types
* find the ASCII text file
* `cat <filename>` reads it

### **Password Found:**

**koReBOKuIDDepwhWk7jZC0RTdopnAYKh**

---

# **🔹 Level 5 → 6**

### **SSH into Level 5**

```
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists folders
* `find . -type f -size 1033c` finds the file
* `cat ./maybehere07/.file2` reads it

### **Password Found:**

**DXjZPULLxYr17uwoI01bNLQbtFemEgo7**

---

# **🔹 Level 6 → 7**

### **SSH into Level 6**

```
ssh bandit6@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `ls` lists contents
* `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null` finds correct file
* `cat <path>` prints password

### **Password Found:**

**HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs**

---

# **🔹 Level 7 → 8**

### **SSH into Level 7**

```
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `grep "millionth" data.txt` finds the correct line

### **Password Found:**

**cvX2JJa4CFALtqS87jk27qwqGhBM9plV**

---

# **🔹 Level 8 → 9**

### **SSH into Level 8**

```
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `sort data.txt | uniq -u` prints the unique line

### **Password Found:**

**UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR**

---

# **🔹 Level 9 → 10**

### **SSH into Level 9**

```
ssh bandit9@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `strings data.txt | grep "==="` finds the password string

### **Password Found:**

**truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk**

---

# **🔹 Level 10 → 11**

### **SSH into Level 10**

```
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `base64 -d data.txt` decodes Base64

### **Password Found:**

**IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR**

---

# **🔹 Level 11 → 12**

### **SSH into Level 11**

```
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

### Commands Used

* `cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'` decodes ROT13

### **Password Found:**

**5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu**

---


