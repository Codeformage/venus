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
User mia has left her password in the file -
**Solution:**  <br>
cat ./- <br>
***iKXIYg0pyEH2Hos***

---
**5º Chanllenge:**
***Task:*** <br> 
It seems that the user camila has left her password inside a folder called hereiam
**Solution:**  <br>
 find / -type d -name hereiam <br>
 ls -a /opt/hereiam <br>
 cat /opt/hereiam/.here <br>
***F67aDmCAAgOOaOc***

---

**6º Chanllenge:**
***Task:*** <br> 
The user luna has left her password in a file inside the muack folder.
**Solution:**  <br>
 find ~ <br>
 cat ./muack/111/111/muack <br>
***j3vkuoKQwvbhkMc***

---

**7º Chanllenge:**
***Task:*** <br> 
The user eleanor has left her password in a file that occupies 6969 bytes.
**Solution:**  <br>
find / -size 6969c 2>/dev/null <br>
cat /usr/share/moon.txt <br>
***UNDchvln6Bmtu7b***

---

**8º Chanllenge:**
***Task:*** <br> 
The user victoria has left her password in a file in which the owner is the user violin.
**Solution:**  <br>
find / -user violin <br>
cat /usr/local/games/yo <br>
***pz8OqvJBFxH0cSj***

---

**9º Chanllenge:**
***Task:*** <br> 
The user isla has left her password in a zip file.
**Solution:**  <br>
vim paswOrd.zip <br>

***D3XTob0FUImsoBb***

---

**10º Chanllenge:**
***Task:*** <br> 
The password of the user lucy is in the line that ends with 0JuAZ (these last 5 characters are not part of her password)
**Solution:**  <br>
grep '^a9HFX' <br>

***WKINVzNQLKLDVAc***

---

