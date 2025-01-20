# Scripting

Learning scripting basics is an excellent step toward automating tasks and working more efficiently with the terminal. Let's dive into the essentials of scripting, specifically focusing on shell scripting, which is common on Linux and macOS.

---

### **What is Shell Scripting?**
A **shell script** is a text file containing a series of commands that the shell (e.g., Bash, Zsh) executes. It’s like writing a "to-do list" for the terminal.

---

### **Steps to Create and Run a Shell Script**

1. **Create a Script File**:
   - Use a text editor (e.g., `nano`, `vim`, or `touch`) to create a new file.
   - Example:
     ```bash
     nano script.sh
     ```

2. **Add the Shebang**:
   - The first line of your script should specify the interpreter.
   - Example:
     ```bash
     #!/bin/bash
     ```
   - This tells the system to use the Bash shell to execute the script.

3. **Write Commands**:
   - Add terminal commands to the file, one per line.
   - Example:
     ```bash
     #!/bin/bash
     echo "Hello, World!"
     ```

4. **Make the Script Executable**:
   - Use the `chmod` command to give execution permission.
   - Example:
     ```bash
     chmod +x script.sh
     ```

5. **Run the Script**:
   - Execute the script by typing:
     ```bash
     ./script.sh
     ```

---

### **Basic Concepts in Shell Scripting**

#### **1. Variables**
Store and reuse values.
- Example:
  ```bash
  #!/bin/bash
  name="Kaelo"
  echo "Hello, $name!"
  ```

#### **2. Conditional Statements**
Add logic to your scripts.
- Example:
  ```bash
  #!/bin/bash
  if [ $1 -eq 10 ]; then
    echo "The number is 10."
  else
    echo "The number is not 10."
  fi
  ```

#### **3. Loops**
Repeat tasks.
- **For Loop**:
  ```bash
  #!/bin/bash
  for i in {1..5}; do
    echo "Number: $i"
  done
  ```
- **While Loop**:
  ```bash
  #!/bin/bash
  count=1
  while [ $count -le 5 ]; do
    echo "Count: $count"
    ((count++))
  done
  ```

#### **4. Functions**
Organize code into reusable blocks.
- Example:
  ```bash
  #!/bin/bash
  greet() {
    echo "Hello, $1!"
  }
  greet "Kaelo"
  ```

#### **5. Input and Output**
- Read user input:
  ```bash
  #!/bin/bash
  echo "Enter your name:"
  read name
  echo "Hello, $name!"
  ```

---

### **Tips for Writing Scripts**

- **Use Comments**:
  Explain your code using `#`:
  ```bash
  # This script greets the user
  echo "Hello, World!"
  ```

- **Debugging**:
  Add `set -x` at the top of your script to debug step by step.

- **Test in Small Parts**:
  Run small sections of your script to ensure they work as expected.

- **Organize Scripts**:
  Save your scripts in a dedicated directory, like `~/scripts`.

---

### **Practice Challenge**
Create a script that:
1. Greets the user.
2. Asks for their favorite number.
3. Checks if it’s greater than 10 or not.
4. Outputs an appropriate message.

Example solution:
```bash
#!/bin/bash
echo "Welcome to the script!"
echo "What is your favorite number?"
read number

if [ $number -gt 10 ]; then
  echo "Wow, $number is a big number!"
else
  echo "$number is a nice choice!"
fi
```

