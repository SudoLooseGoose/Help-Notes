
# Copy, Move, Remove

Commands to be able to copy, move, remove directorys and files from within PowerShell CLI

---
---

***Copy***

---

Files

- WIll copy to specified directory

> `Copy-Item "C:\\path-to\file.type or file.type" -Destination "C:\\path-to\new-file.type or new-file.type`

Directorys

---

- Will copy directory to an existing directory
    
> `Copy-Item -Path "C:\directory-name\path or directory name" -Destination "C:\new-path\to-existing-directory" -Recurse`

- Will copy directory to a new directory

> `Copy-Item -Path "C:\directory-name -Destination "C:\path-to\new-dirctory
