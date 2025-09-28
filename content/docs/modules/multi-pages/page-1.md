---
title: Page 1
description: "Quick reference of commands, patterns, tips"
---

# Developer Cheatsheet

Useful commands, patterns, and remiders for daily works.

---

## Essentials

### Git

| Command | What It Does | Note |
| --- | --- | --- |
| `git status` | Show working directory status | Use often |
| `git add <file>` | Stage a file for commit | Or `git add . ` to add all changes |
| `git commit -m "msg"` | Commit staged changes | Write meaningful messages |
| `git log --oneline -graph` | Show compact commit history | Greate for reviewing branch work |
| `git rebase -i HEAD~3` | Interactive rebase last 3 commits | Use to squash / fix mistakes |

### Bash / Shell

```bash
# Navigate
cd /path/to/project

# List hidden files
ls -la

# Search in files
grep -R "TODO" .

# Start simple HTTP server (Python3)
python3 -m http.server 8000
```

### Ruby code
```ruby
puts "Hello world!"
```

### Golang code

```go
package main

import fmt

function main() {
    fmt.Println("Hello world!!!")
}
```

### JavaScript

```js
let message = "Hello, World!";
const pi = 3.14159;

console.log(message);
console.log("The value of Pi is: " + pi);
```
