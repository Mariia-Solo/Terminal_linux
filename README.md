# Terminal_linux

**1)Linux terminal (GitBash) commands**

**2) Создать папку:** mkdir group_22

**3) Зайти в папку :** cd group_22/

**4) Создать 3 папки :** 
mkdir papka1
mkdir papka2
mkdir papka

**5) Зайти в любую папку :**
cd papka1/

**6) Создать 5 файлов (3 txt, 2 json) :**
touch 1_txt.file.txt
touch 2_txt.file.txt
touch 3_txt.file.txt
touch 1_json.file.json
touch 2_json.file.json

**7) Создать 3 папки :**
mkdir P1
mkdir P2
mkdir P3

**8. Вывести список содержимого папки :**
ls -la

**9) + Открыть любой txt файл:**
vim 1_txt.file.txt
для редактирования жмем I (insert)

**10) + написать туда что-нибудь, любой текст :**
Пишем текст Hello!

**11) + сохранить и выйти:**
esc, затем  :wq

**12) Выйти из папки на уровень выше :**
cd ../

**13) переместить любые 2 файла, которые вы создали, в любую другую папку.**

mv /Users/mary/group_22/papka1/1_txt.file.txt /Users/mary/group_22/

mv /Users/mary/group_22/papka1/2_txt.file.txt /Users/mary/group_22/

Для одновременного перемещения файлов используем фигурные скобки {} :

mv /Users/mary/group_22/papka1/{2_txt.file.txt,1_txt.file.txt}  /Users/mary/group_22/
 
**14) скопировать любые 2 файла, которые вы создали, в любую другую папку.**
cp 1_txt.file.txt /Users/mary/group_22/papka2/

cp 2_txt.file.txt /Users/mary/group_22/papka2/

Для одновременного копирования нескольких файлов используем фигурные скобки {} :

cp {1_txt.file.txt, 2_txt.file.txt} /Users/mary/group_22/papka2/

**15) Найти файл по имени:**

sudo find ./ -type f -name "*1_txt.file.txt"

**16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. :**
tail -f 1_txt.file.txt 

**17) вывести несколько первых строк из текстового файла**
head -n3 /Users/mary/group_22/1_txt.file.txt

**18) вывести несколько последних строк из текстового файла**
tail -n2 /Users/mary/group_22/1_txt.file.txt

**19) просмотреть содержимое длинного файла (команда less) изучите как она работает :**
 less 1_txt.file.txt 
чтобы выйти, нажать Q

**20) вывести дату и время:**
date

=========

**Задание*.**
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000

curl "http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000"
