## Storage Management commnds
[File and Directory commands]


*   **Why we need directories/folders?**
    *   It is a way to organize or group related files.
    *   They help in locating files easily on a storage device among many other files.
    *   A directory always contains files inside it.

*   **How to create a directory?**
    *   Use the command: `mkdir directoryName`
    *   This creates a directory with the specified name under the current directory.
    *   Use the command: `ls directoryName` to see the contents of a directory.
*   **`cd directoryName`**
    *   Used to change to the newly created directory.

*   **Special Directory References**
    *   **`.`** (a single dot) refers to the current location/directory.
    *   **`..`** (two dots) refers to the parent of the current directory.

*   **`cd ..`**
    *   Takes you to the parent directory of the current directory.

*   **`cd`** (without any input)
    *   Takes you to the home directory of the user (e.g., `/home/username`).

*   **`cd ~`**
    *   The tilde (`~`) always refers to the home directory location of the user.
    *   This command also takes you to the home directory.

*   **`cd /dir1/dir2`**
    *   You can navigate through multiple directories at once by specifying the full path separated by slashes (`/`).

*   **`cd -`**
    *   This command will take you back to the previous directory you were in.