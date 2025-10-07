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
The password of the user violet is in the line that begins with a9HFX (these 5 characters are not part of her password.).
**Solution:**  <br>
grep '^a9HFX' <br>

***WKINVzNQLKLDVAc***

---

**11º Chanllenge:**
***Task:*** <br> 
The password of the user lucy is in the line that ends with 0JuAZ (these last 5 characters are not part of her password)
**Solution:**  <br>
grep '0JuAZ$' end <br>

***OCmMUjebG53giud***

---

**12º Chanllenge:**
***Task:*** <br> 
The password of the user elena is between the characters fu and ck
**Solution:**  <br>
grep -oP '(?<=fu).*?(?=ck)' file.yo <br>

***4xZ5lIKYmfPLg9t***

---

**13º Chanllenge:**
***Task:*** <br> 
The user alice has her password is in an environment variable.
**Solution:**  <br>
env

***Cgecy2MY2MWbaqt***

---

**14º Chanllenge:**
***Task:*** <br> 
The admin has left the password of the user anna as a comment in the file passwd.
**Solution:**  <br>
cat /etc/passwd

***w8NvY27qkpdePox***

---

**15º Chanllenge:**
***Task:*** <br> 
Maybe sudo can help you to be natalia.
**Solution:**  <br>
sudo -i -u natalia

******

---

**16º Chanllenge:**
***Task:*** <br> 
The password of user eva is encoded in the base64.txt file
**Solution:**  <br>
echo dXBzQ0EzVUZ1MTBmREFPCg== | base64 --decode

***upsCA3UFu10fDAO***

---

**17º Chanllenge:**
***Task:*** <br> 
The password of the clara user is found in a file modified on May 1, 1968.
**Solution:**  <br>
find / -type f -mtime +$((55*365)) 2>dev>null

***39YziWp5gSvgQN9***

---

**18º Chanllenge:**
***Task:*** <br> 
The password of user frida is in the password-protected zip (rockyou.txt can help you)
**Solution:**  <br>


***Ed4ErEUJEaMcXli***

---

**19º Chanllenge:**
***Task:*** <br> 
The password of eliza is the only string that is repeated (unsorted) in repeated.txt.
**Solution:**  <br>
uniq -d repeated.txt

***Fg6b6aoksceQqB9***

---

**20º Chanllenge:**
***Task:*** <br> 
The user iris has left me her key.v
**Solution:**  <br>
ls -a <br>
ssh -i .iriskey iris@venus 

***kYjyoLcnBZ9EJdz***

---

**21º Chanllenge:**
***Task:*** <br> 
User eloise has saved her password in a particular way.
**Solution:**  <br>
After few revisions I noticed that is coded in base64 and is a jpg file <br>
base64 -d eloise > eloise.jpg  (in local, previously I made a scp) <br>

***yOUJlV0SHOnbSPm***

---

**22º Chanllenge:**
***Task:*** <br> 
User lucia has been creative in saving her password.
**Solution:**  <br>
echo '7576 4d77 4644 5172 5157 504d 6547 500a' | xxd -r -p <br>

***uvMwFDQrQWPMeGP***

---

**23º Chanllenge:**
***Task:*** <br> 
The user isabel has left her password in a file in the /etc/xdg folder but she does not remember the name, however she has dict.txt that can help her to remember.
**Solution:**  <br>
cat dict.txt | xargs -I {} find /etc/xdg/{} -maxdepth 0 2>/dev/null -print <br>

***H5ol8Z2mrRsorC0***

---

**24º Chanllenge:**
***Task:*** <br> 
The password of the user freya is the only string that is not repeated in different.txt
**Solution:**  <br>
uniq -u different.txt cat <br>

***EEDyYFDwYsmYawj***

---

**25º Chanllenge:**
***Task:*** <br> 
User alexa puts her password in a .txt file in /free every minute and then deletes it.
**Solution:**  <br>
while true; do [ -f /free/* ] && cat /free/*; sleep 1; done <br>

***mxq9O3MSxxX9Q3S***

---

**26º Chanllenge:**
***Task:*** <br> 
The password of the user ariel is online! (HTTP)
**Solution:**  <br>
curl localhost <br>

***33EtHoz9a0w2Yqo***

---

**27º Chanllenge:**
***Task:*** <br> 
Seems that ariel dont save the password for lola, but there is a temporal file.
**Solution:**  <br>
opne with vim the .goas.swp and recover it and try every password<br>


VVjqJGRrnfKmcgD No 
bnQgcXYamhSDSff
QsymOOVbzSaKmRm
cbjYGSvqAsqIvdg
LkWReDaaLCMDlLf
DabEJLmAbOQxEnD
mYhQVLDKdJrsIwG
d3LieOzRGX5wud6 Si
EKvJoTBYlwtwFmv no
PEOppdOkSqJZweH no
rSkPlPhymYcerMJ no
GBUguuSpXVjpxLc no
NdnszvjulNellbK no
IaOpTdAuhSjGZnu no
RGBEMbZHZRgXZnu no 
rxhKeFKveeKqpwp no
cOXlRYXtJWnVQEG no
ppkJjqYvSCIyAhK No 

***d3LieOzRGX5wud6***

**28º Chanllenge:**
***Task:*** <br> 
The user celeste has left a list of names of possible .html pages where to find her password.
**Solution:**  <br>
find / -type f -name "*.html" 2>/dev/null | \
awk -F'/' '{gsub(/\.html$/, "", $NF); print $NF}' | \
grep -Ff pages.txt | \
while read PAGE; do
    # Ejecuta curl, obtiene el código de estado y lo guarda en la variable STATUS
    STATUS=$(curl -s -o /dev/null -w "%{http_code}" "http://localhost/${PAGE}.html")
    
    # Compara el código de estado (200 es éxito)
    if [ "$STATUS" -eq 200 ]; then
        echo "http://localhost/$PAGE.html"  # Imprime solo la URL
    fi
done <br>
Only I have to chek index, cebolla and index.nginx-debian.html <br>
lola@venus:~$ curl http://localhost/index.html <br>
33EtHoz9a0w2Yqo <br>
lola@venus:~$ curl http://localhost/cebolla.html <br>
VLSNMTKwSV2o8Tn <br>

***VLSNMTKwSV2o8Tn***

---

**29º Chanllenge:**
***Task:*** <br> 
The user celeste has access to mysql but for what? <br>
**Solution:**  <br>
<br>

***mxq9O3MSxxX9Q3S***
MariaDB [venus]> SELECT * FROM people;
+-----------+---------------+--------------------------------+
| id_people | uzer          | pazz                           |
+-----------+---------------+--------------------------------+
|         1 | nuna          | ixpfdsvcxeqdW                  |
|         2 | nona          | ixpvcxvcxeqdW                  |
|         3 | manue         | ixpfdsfdseqdW                  |
|         4 | samoa         | ixperrewrweqdW                 |
|         5 | dsaewq        | ixpefdsfsqdW                   |
|         6 | fdsfewrew     | ixpedvcxv4qdW                  |
|         7 | koiuoiudsadas | ixpredsfdeqdW                  |
|         8 | vcxfdsfew     | ixp342432eqdW                  |
|         9 | dasd          | ixpeiuyiuyqdW                  |
|        10 | helen         | uytuytjhgixpeqdW               |
|        11 | tudou         | ijhgjghxpeqfdfsfddW            |
|        12 | fdsoiurew     | ixpfdsfsdsvcxvcxeqdW           |
|        13 | inan          | imbnmnbxpeqdW                  |
|        14 | zkret         | ixpeqkjhkhjkdW                 |
|        15 | cjhcx         | i432423xpeqdW                  |
|        16 | sfdfdsml      | ixpeqdsfsdfdsfW                |
|        17 | svcxvcxml     | 432423ixpeqdW                  |
|        18 | xml           | ixpejhgjhgqdW                  |
|        19 | pdf           | ixperewrewrewqdW               |
|        20 | txt           | ixpeuytuytqdW                  |
|        21 | vcxvcx        | ixpefdsfdsfdfdsqdW             |
|        22 | dsadsa        | ixpeqdjhkjhW                   |
|        23 | lel           | ixpvcxvcxvcxeqdW               |
|        24 | lul           | ixpeqdmnbmnbmnbmW              |
|        25 | dog           | ixperewrewrewqdW               |
|        26 | cat           | ixvcxvdsfsdvpeqdW              |
|        27 | pet           | ixiufohsyuoirewpeqdW           |
|        28 | pzzz          | ixvcxvcxvpeqdW                 |
|        29 | ls            | ixpehgfdhdhqdW                 |
|        30 | vi            | ixpetrvvrqdW                   |
|        31 | tmux          | iuovcxoiujvcxixpeqdW           |
|        32 | screen        | ixpeqrewregfdgdW               |
|        33 | yes           | ixpebvcgdfgqdW                 |
|        34 | nop           | ixpefdsqdW                     |
|        35 | haha          | 8===xKmPDsJSKpHLzkqKXyjx===D~~ |
|        36 | love          | ixpegfdgqdW                    |
|        37 | dsadsa        | fdsvcxvcxixpeqdW               |
|        38 | d4t4          | erwerewreixpeqdW               |
|        39 | nna           | gdfgdixpeqdW                   |
|        40 | nin           | aaafdixpeqdW                   |
|        41 | tre           | fdsafixpeqdW                   |
|        42 | tfas          | igfdgfdgxpeqdW                 |
|        43 | zcxc          | ixfdgdfgpeqdW                  |
|        44 | yuio          | ixpgbvcbvcbeqdW                |
|        45 | jhgyurtrt     | treterterixpeqdW               |
|        46 | lodsa         | itreterxpeqdW                  |
|        47 | zarah         | ixpvcbvcbeqdW                  |
|        48 | zkkad         | ixpedfgvbcxbvcqdW              |
|        49 | bvher         | vcxvcxgfdgfdixpeqdW            |
|        50 | dsadsa        | ixpeqergdfwer32dW              |
|        51 | ch4rm         | ixpeewf23qdW                   |
|        52 | Aza           | ixpjhgjgheqdW                  |
|        53 | avij          | ixpegfdgdfgqdW                 |
|        54 | crom          | ixpefdbvvcbrqdW                |
|        55 | bubu          | ixpetretretqdW                 |
|        56 | bebe          | ixpeghfgfdqdW                  |
|        57 | baba          | ixpeffesfqdW                   |
|        58 | bael          | ixpesdvsdvsdqdW                |
|        59 | vaze          | ixpe23r23rf23qdW               |
|        60 | upper         | ixpe43r43rqdW                  |
|        61 | loz           | ixpeqddfsdW                    |
|        62 | mind          | ixpfsdfsdfsdeqdW               |
|        63 | mymy          | ixpevcxvqdW                    |
|        64 | ina           | ixpee23e32rqdW                 |
|        65 | ein           | ixpejytjytjhgjqdW              |
|        66 | n1n4          | ixpehgjghjhghgqdW              |
|        67 | where         | ixljkgjgpeqdW                  |
|        68 | you           | ixpeqdhggjhgjW                 |
|        69 | are           | ixVCXVCXVCXVCXdW               |
|        70 | what          | ixpeqhgjggdW                   |
|        71 | dsaqqqqqq     | ixpeqVCXVCXdW                  |
|        72 | h0j3n         | ixpemnbmbnmghqdW               |
|        73 | nana          | ixpeqVSDFWCdW                  |
|        74 | nina          | ixpeqdWuvC5N9kG                |
|        75 | nunu          | ixpeSFDSFDSVCXqdW              |
|        76 | fdse          | ixpeDFSWEF2qdW                 |
|        77 | dsar          | ixpeF43F3F34qdW                |
|        78 | yop           | ixpeqdWCSDFDSFD                |
|        79 | loco          | ixpeF43F34F3qdW                |
|        80 | zaza          | ixpeYUTHNYGTHYTqdW             |
|        81 | jhon          | ixpeFDSJYTUJTYqdW              |
|        82 | tell          | ixpeHYTTqdW                    |
|        83 | ma            | uyixptje4FSFWEFqdW             |
|        84 | mum           | jghixpeqdW                     |
|        85 | nanaa         | 432432ixpeqdW                  |
|        86 | nnnniinn      | irewxpeqdW                     |
|        87 | iourewoiure   | rewixpeqdW                     |
|        88 | lkjfdsoiu     | dsaixpeqdW                     |
|        89 | vcxnoj        | dasdasixpeqdW                  |
|        90 | ioyuwer       | ixpeqdvcxvcxW                  |
|        91 | kaka          | ixpeqdW                        |
|        92 | nini          | ixpeqdvcxW                     |
|        93 | zong          | ixpeqdWfdsfsdf                 |
|        94 | nana          | ixpefdsafdsqdW                 |
|        95 | ninna         | ixpeqOPUIFDSFDSdW              |

with hydra tested all user and passwords and nina was the one <br>

***ixpeqdWuvC5N9kG***

--- 


