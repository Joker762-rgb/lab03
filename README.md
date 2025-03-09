luka@luka-VirtualBox:~$ cd ~/Joker762-rgb/workspace/projects/lab02
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ touch .gitignore
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git add .gitignore
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git commit -m"added .gitignore"
[master fb42a9c] added .gitignore
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Joker762-rgb
Password for 'https://Joker762-rgb@github.com': 
Перечисление объектов: 3, готово.
Подсчет объектов: 100% (3/3), готово.
При сжатии изменений используется до 12 потоков
Сжатие объектов: 100% (2/2), готово.
Запись объектов: 100% (2/2), 268 байтов | 268.00 КиБ/с, готово.
Всего 2 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
To https://github.com/Joker762-rgb/lab02.git
   f060301..ae249fd  master -> master
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git pull origin master
remote: Enumerating objects: 35, done.
remote: Counting objects: 100% (35/35), done.
remote: Compressing objects: 100% (28/28), done.
remote: Total 35 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
Распаковка объектов: 100% (35/35), 11.89 КиБ | 193.00 КиБ/с, готово.
Из https://github.com/Joker762-rgb/lab02
 * branch            master     -> FETCH_HEAD
 * [новая ветка]     master     -> origin/master
Обновление ae253fd..25f9b86
Fast-forward
 .gitignore | 4 ++++
 1 file changed, 4 insertions(+)
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git log
commit fb42a9c95991dd0241cad91838c97255779c685e (HEAD -> master)
Author: Joker762-rgb <Kuzmin2006.ru@yandex.ru>
Date:   Sun Mar 9 13:23:21 2025 +0300

    added .gitignore

commit 71a1cb3222cf398bcd46ee7134ea76f18ac2aa8f
Author: Joker762-rgb <Kuzmin2006.ru@yandex.ru>
Date:   Sun Mar 2 16:56:48 2025 +0300

    added sources

commit c0e557027e2f61919b2dfef3d8cb0f0d58ef9995
Author: Joker762-rgb <Kuzmin2006.ru@yandex.ru>
Date:   Sun Mar 2 16:44:30 2025 +0300

    added README.md
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ mkdir sources
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ mkdir include
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ mkdir examples
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ cat > sources/print.cpp << EOF
> #include<print.hpp>
> void print(const std::string& text, std::ostreasm& out) {
> out << text;
> }
> void print(const std::string& text, std::ofstream& out) {
> out << text;
> }
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ cat > include/print.hpp << EOF
> #include<fstream>
> #include<iostream>
> #include<string>
> void print(const std::string& text, std::ofstream& out);
> void print(const std::string& text, std::ostream& out = std::cout);
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ cat > examples/example1.cpp << EOF
> #include<print.hpp>
> int main(int argc, char** argv) {
> print("hello");
> }
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ cat > examples/example2.cpp << EOF
> #include<print.hpp>
> #include<fstream>
> int main(int argc, char** argv) {
> std::ofstream file("log.txt");
> print(std::string("hello"), file);
> }
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ edit README.md
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git status
Текущая ветка: master
Неотслеживаемые файлы:
  (используйте «git add <файл>...», чтобы добавить в то, что будет включено в коммит)
	     examples/
       include/
       sources/
индекс пуст, но есть неотслеживаемые файлы
  (используйте «git add», чтобы проиндексировать их)
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git add .
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git commit -m"added sources"
[master ec0325e] added sources
  4 files changed, 24 insertions(+)
   create mode 100644 examples/example1.cpp
   create mode 100644 examples/example2.cpp
   create mode 100644 include/print.hpp
   create mode 100644 sources/print.cpp
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Joker762-rgb
Password for 'https://Joker762-rgb@github.com': 
Перечисление объектов: 10, готово.
Подсчет объектов: 100% (10/10), готово.
При сжатии изменений используется до 12 потоков
Сжатие объектов: 100% (7/7), готово.
Запись объектов: 100% (9/9), 874 байтов | 874.00 КиБ/с, готово.
Всего 9 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
To https://github.com/Joker762-rgb/lab02.git
   26f9b86..773b80c  master -> master
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab02$ 
