# 🚀 Venus HackMyVM

In this file is described the progress of the learning challenge in Venus.

Basic connection: ssh hacker@venus.hackmyvm.eu -p 5000

---

**1º Chanllenge:**
***Task:*** <br> 
User sophia has saved her password in a hidden file in this folder. Find it and log in as sophia <br>
**Solution:**  <br>
ls -a for hidden files  <br>
***Y1o645M3mR84ejc***

---

**2º Chanllenge:**
***Task:*** <br> 
The user angela has saved her password in a file but she does not remember where ... she only remembers that the file was called whereismypazz.txt
**Solution:**  <br>
find / -name whereismypazz.txt 2>/dev/null <br>
***oh5p9gAABugHBje***

---

**3º Chanllenge:**
***Task:*** <br> 
The password of the user emma is in line 4069 of the file findme.txt
**Solution:**  <br>
sed -n '4069p' findme.txt <br>
***fIvltaGaq0OUH8O***

---

**4º Chanllenge:**
***Task:*** <br> 
The password of the user emma is in line 4069 of the file findme.txt
**Solution:**  <br>
sed -n '4069p' findme.txt <br>
***fIvltaGaq0OUH8O***

---
