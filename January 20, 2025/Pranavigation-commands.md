Here are some examples of commonly used terminal navigation commands along with their descriptions:

---

### **Basic Navigation Commands**
1. **`pwd`** (Print Working Directory)  
   - **Example**:  
     ```
     pwd
     ```
     - Displays the current directory you are in.
     - Output might be: `/home/kaelo/projects`

2. **`ls`** (List Files)  
   - **Examples**:  
     ```
     ls
     ls -l   # List files with detailed information
     ls -a   # Include hidden files
     ls -lh  # Display file sizes in human-readable format
     ```
     - Lists files and directories in the current directory.

3. **`cd`** (Change Directory)  
   - **Examples**:  
     ```
     cd /home/kaelo/projects  # Navigate to a specific directory
     cd ..                    # Go up one directory level
     cd ~                     # Go to your home directory
     cd /                     # Go to the root directory
     ```
     - Moves between directories.

4. **`ls` with `cd`**  
   - Combine `ls` to check contents and `cd` to navigate:  
     ```
     ls
     cd documents
     ```

---

### **Advanced Navigation**
1. **Navigate Multiple Levels**  
   - **Example**:  
     ```
     cd ~/projects/my-app/src
     ```
     - Moves directly to a deeply nested directory.

2. **Use Tab for Auto-Completion**  
   - **Example**:  
     ```
     cd ~/proj<TAB>
     ```
     - Typing a partial name and pressing Tab auto-completes the directory name.

3. **Go Back to the Previous Directory**  
   - **Example**:  
     ```
     cd -
     ```
     - Switches back to the directory you were just in.

4. **List Directory Contents Recursively**  
   - **Example**:  
     ```
     ls -R
     ```
     - Lists all files and directories, including their subdirectories.

---

### **Directory Management**
1. **Create a New Directory**  
   - **Example**:  
     ```
     mkdir my_new_project
     ```
     - Creates a directory named `my_new_project`.

2. **Navigate into a New Directory Immediately**  
   - **Example**:  
     ```
     mkdir my_new_project && cd my_new_project
     ```
     - Creates and enters the directory in one command.

3. **Check Path Using `realpath`**  
   - **Example**:  
     ```
     realpath my_new_project
     ```
     - Displays the absolute path of the directory or file.

---

### **Additional Tips**
- **`tree` Command**: Visualize the directory structure.  
   ```
   tree
   ```
   *(Note: You may need to install this command on some systems.)*

- **`man` Command**: Learn more about commands.  
   ```
   man cd
   ```
   *(Displays the manual page for `cd`.)*
