**Supported File System Types in Linux:**

Linux supports many types of file systems. Some of the common ones include:

1. **ext (Extended File System)** – The first version, now outdated.
2. **ext2 (Second Extended File System)** – Improved version of ext; does not support journaling.
3. **ext3 (Third Extended File System)** – Like ext2 but adds journaling for better recovery after crashes.
4. **ext4 (Fourth Extended File System)** – Faster and supports larger files and volumes. Commonly used now.
5. **JSF** – This seems to be a typo; maybe you meant **JFS (Journaled File System)** by IBM.
6. **XFS** – High-performance journaling file system, good for handling large files.
7. **Btrfs (B-tree File System)** – Modern file system with advanced features like snapshots and pooling.

---

**Linux File System is a Hierarchical File System:**

* The Linux file system is organized like a tree.
* It starts with a **root** directory called `/` (a single slash).
* All other directories are **inside** this root directory.
* It’s called **hierarchical** because it has a parent-child relationship like folders inside folders.

---

**Basic Linux Directories (in simple words):**

* `/` = Root directory. The top of the Linux file system.
* `/bin` = Contains basic Linux commands like `ls`, `cp`, `rm`.
* `/boot` = Files needed to start (boot) the computer, like the Linux kernel.
* `/dev` = Stands for "devices"; shows your hardware (like USB drives, hard disks) as files.
* `/mnt` = Used to temporarily mount external storage or remote systems.
* `/media` = Used to mount removable media like CDs, USBs, headphones.
* `/usr` = Programs and software that can be used by all users.
* `/proc` = Contains info about running processes, shown as files.
* `/lib` = Libraries (like helpers for programs) that many applications use.
* `/tmp` = Temporary files are stored here. Automatically cleared.
* `/var` = Variable files like logs, print jobs, or big data files.
* `/etc` = System configuration files. Settings for services and software.
* `/opt` = Optional software installed by the user or third-party apps.
* `/sbin` = System commands for the **superuser (root user)**.
* `/home` = Each normal user gets their own folder here.
  Example: `/home/anil` is the personal folder for a user named **anil**.

---
