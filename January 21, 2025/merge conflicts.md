### **How to Resolve Merge Conflicts in Git** 🚀  

Merge conflicts happen when Git can't automatically combine changes from different branches. This usually happens when:  
✅ Two people edit the same line of a file.  
✅ A file is deleted in one branch but modified in another.  
✅ The same file is modified in different branches.  

---

## **1. Identify the Merge Conflict**  
When you try to merge a branch:  
```sh
git merge feature-branch
```
Git will show a message like:  
```
CONFLICT (content): Merge conflict in file.txt
Automatic merge failed; fix conflicts and commit the result.
```

---

## **2. Open the Conflict File**  
Git marks the conflicting parts in the file like this:  

```txt
<<<<<<< HEAD
This is the version from your current branch.
=======
This is the version from the branch being merged.
>>>>>>> feature-branch
```

---

## **3. Resolve the Conflict Manually**  
- **Keep one version** or **combine both**.  
- Remove `<<<<<<<`, `=======`, and `>>>>>>>`.  

### **Example Resolution:**  
Before:  
```txt
<<<<<<< HEAD
This is the original text.
=======
This is the updated text from feature-branch.
>>>>>>> feature-branch
```
After fixing:  
```txt
This is the updated text from feature-branch.
```

---

## **4. Mark the Conflict as Resolved**  
After fixing all conflicts, **stage the file**:  
```sh
git add file.txt
```

Then **commit the resolution**:  
```sh
git commit -m "Resolved merge conflict in file.txt"
```

Finally, **push the changes**:  
```sh
git push origin main
```

---

## **5. Abort the Merge (If Necessary)**  
If you want to cancel the merge and start over:  
```sh
git merge --abort
```

---

### **Best Practices to Avoid Merge Conflicts**  
✅ **Pull latest changes before working**  
```sh
git pull origin main
```  
✅ **Use branches for new features**  
```sh
git checkout -b new-feature
```  
✅ **Communicate with your team** to avoid conflicts  

