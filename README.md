```markdown
# 0x00. Shell, Navigation

## Overview

This project focuses on fundamental shell navigation and file manipulation tasks within a Linux environment. It covers essential commands for creating, copying, renaming, moving, and deleting files and directories. This project is designed to build a strong foundation in basic command-line operations, crucial for any system administrator or developer working with Linux-based systems.

## Project Structure

This repository contains the scripts or commands used to complete the following tasks:

-   **0. Create me!**: Creating an empty file.
-   **1. More of me**: Copying a file to another location.
-   **2. To old**: Renaming a file within the same directory.
-   **3. Not here**: Moving a file to a different directory.
-   **4. Not anymore**: Deleting a file.
-   **5. Organization is key!**: Creating a new directory.
-   **6. No need**: Removing an empty directory.

## Tasks and Implementation

### 0. Create me!

-      **Objective**: Create an empty file named `so_cool` in the `/root` directory.
-   **Implementation**:
    ```bash
    cd /root
    touch so_cool
    ls
    ```
-   **Verification**: The `ls` command confirms the creation of the `so_cool` file.

### 1. More of me

-   **Objective**: Copy the file `school` from `/root` to `/tmp`.
-   **Implementation**:
    ```bash
    cd /root
    cp school /tmp
    ls /tmp
    ```
-   **Verification**: The `ls /tmp` command verifies the presence of the copied `school` file in the `/tmp` directory.

### 2. To old

-   **Objective**: Rename the file `old_school` to `new_school` within the `/root` directory.
-   **Implementation**:
    ```bash
    cd /root
    mv old_school new_school
    ls
    ```
-   **Verification**: The `ls` command shows the renamed file `new_school`.

### 3. Not here

-   **Objective**: Move the file `not_here` from `/root` to `/tmp/right_school`.
-   **Implementation**:
    ```bash
    cd /root
    mv not_here /tmp/right_school
    ls /tmp/right_school
    ```
-   **Verification**: The `ls /tmp/right_school` command confirms the file's new location.

### 4. Not anymore

-   **Objective**: Delete the file `ready_to_be_removed` from `/root`.
-   **Implementation**:
    ```bash
    cd /root
    rm ready_to_be_removed
    ls
    ```
-   **Verification**: The `ls` command verifies the file's absence.

### 5. Organization is key!

-   **Objective**: Create a directory named `school_is_amazing` in `/root`.
-   **Implementation**:
    ```bash
    cd /root
    mkdir school_is_amazing
    ls -d school_is_amazing
    ```
-   **Verification**: The `ls -d school_is_amazing` command confirms the directory's creation.

### 6. No need

-   **Objective**: Remove the empty directory `empty_directory` from `/root`.
-   **Implementation**:

    ```bash
    cd /root
    rmdir empty_directory
    ls -d empty_directory 2>/dev/null; echo $?
    ```

-   **Verification**: The exit code of the `ls -d empty_directory` command being non-zero confirms the directories deletion.

## Usage

These tasks are designed to be executed within a Linux shell environment. Access to a command-line interface is required. The commands provided can be directly copied and pasted into the terminal.

## Learning Objectives

-      Understanding and using basic shell commands for file and directory manipulation.
-      Navigating the file system using the command line.
-      Developing proficiency in creating, copying, renaming, moving, and deleting files and directories.
-   Understanding how to verify the results of commands using commands like `ls`.

## Author

Merlyn Zawadi
