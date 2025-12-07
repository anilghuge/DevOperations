- File is a data structure in which we hold the physical address location of the actual data resides on the storage device.

- If we hold address locations of the memory in a file directly we end up in storing address in memory than actual data and storage space will not be used efficiently.

- To avoid the above problem the physical storage has been divided into blocks of sequential memory locations and blocks are assigned to the files and block no's are stored in file to track the information.

- Each block size is fixed so that we can keep block no in a file as a pointer and can save memory for storing the blocks information. For a given file multiple blocks can be assigned depends on the information/data we want to store.

- A file always holds array of block no's pointing to memory locations of the data.

- There are multiple File Systems available for storing and organizing the data on storage devices. The technic/mechanism or algorithmic approach of organizing and storing the data on the storage device will be different from one filesystem to another.

- We can say File System is an integral part of an operating system. Since an operating system should be able to store the data on the physical storage device based on the File System Technic.

- Usually we pick a File System while installing the Operating System because of the above reason.

- We can say indirectly Operating System Vendors comes up with FileSystem Technics as those are integral part.

- Windows Operating System 
    - 1. FAT32(File Allocation Table)
    - 2. NTFS(Network File System)

- MAC 
    - 1. HFS(Hierarchical File System)

- Linux
   - 1. **ext (Extended File System)** – The first version, now outdated.
   - 2. **ext2 (Second Extended File System)** – Improved version of ext; does not support journaling.
   - 3. **ext3 (Third Extended File System)** – Like ext2 but adds journaling for better recovery after crashes.
   - 4. **ext4 (Fourth Extended File System)** – Faster and supports larger files and volumes. Commonly used now.
    - 5. **JSF** – This seems to be a typo; maybe you meant **JFS (Journaled File System)** by IBM.
    - 6. **XFS** – High-performance journaling file system, good for handling large files.
    - 7. **Btrfs (B-tree File System)** – Modern file system with advanced features like snapshots and pooling.