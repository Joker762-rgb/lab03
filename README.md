luka@luka-VirtualBox:~$ export GITHUB_USERNAME=Joker762-rgb
luka@luka-VirtualBox:~$ cd ${GITHUB_USERNAME}/workspace
luka@luka-VirtualBox:~/Joker762-rgb/workspace$ pushd .
~/Joker762-rgb/workspace ~/Joker762-rgb/workspace
luka@luka-VirtualBox:~/Joker762-rgb/workspace$ source scripts/activate
luka@luka-VirtualBox:~/Joker762-rgb/workspace$ git clone https://github.com/Joker762-rgb/lab02.git projects/lab03
Клонирование в «projects/lab03»...
remote: Enumerating objects: 35, done.
remote: Counting objects: 100% (35/35), done.
remote: Compressing objects: 100% (28/28), done.
Получение объектов: 100% (35/35), 11.91 КиБ | 321.00 КиБ/с, готово.
remote: Total 35 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
Определение изменений: 100% (7/7), готово.
luka@luka-VirtualBox:~/Joker762-rgb/workspace$ cd projects/lab03
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git remote remove origin
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git remote add origin https://github.com/Joker762-rgb/lab03.git
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ -std=c++11 -I./include -c sources/print.cpp
Команда «g++» не найдена, но может быть установлена с помощью:
sudo apt install g++
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ sudo apt install g++
[sudo] пароль для luka: 
К установке:                                                      
  g++

Зависимости к установке:
  g++-14  g++-14-x86-64-linux-gnu  g++-x86-64-linux-gnu  libstdc++-14-dev

Предлагаемые пакеты:
  g++-multilib  g++-14-multilib  gcc-14-doc  libstdc++-14-doc

Сводка:
  К обновлению: 0, К установке: 5 К удалению: 0, Не обновляется: 133
  Размер загрузки: 15,9 MB
  Места необходимо: 61,3 MB / 13,4 GB доступно

Продолжить? [Д/н] д
Пол:1 http://ru.archive.ubuntu.com/ubuntu oracular/main amd64 libstdc++-14-dev amd64 14.2.0-4ubuntu2 [2 501 kB]
Пол:2 http://ru.archive.ubuntu.com/ubuntu oracular/main amd64 g++-14-x86-64-linux-gnu amd64 14.2.0-4ubuntu2 [13,4 MB]
Пол:3 http://ru.archive.ubuntu.com/ubuntu oracular/main amd64 g++-14 amd64 14.2.0-4ubuntu2 [19,0 kB]
Пол:4 http://ru.archive.ubuntu.com/ubuntu oracular/main amd64 g++-x86-64-linux-gnu amd64 4:14.1.0-2ubuntu1 [966 B]
Пол:5 http://ru.archive.ubuntu.com/ubuntu oracular/main amd64 g++ amd64 4:14.1.0-2ubuntu1 [1 100 B]
Получено 15,9 MB за 14с (1 166 kB/s)                                           
Выбор ранее не выбранного пакета libstdc++-14-dev:amd64.
(Чтение базы данных … на данный момент установлено 158614 файлов и каталогов.)
Подготовка к распаковке …/libstdc++-14-dev_14.2.0-4ubuntu2_amd64.deb …
Распаковывается libstdc++-14-dev:amd64 (14.2.0-4ubuntu2) …
Выбор ранее не выбранного пакета g++-14-x86-64-linux-gnu.
Подготовка к распаковке …/g++-14-x86-64-linux-gnu_14.2.0-4ubuntu2_amd64.deb …
Распаковывается g++-14-x86-64-linux-gnu (14.2.0-4ubuntu2) …
Выбор ранее не выбранного пакета g++-14.
Подготовка к распаковке …/g++-14_14.2.0-4ubuntu2_amd64.deb …
Распаковывается g++-14 (14.2.0-4ubuntu2) …
Выбор ранее не выбранного пакета g++-x86-64-linux-gnu.
Подготовка к распаковке …/g++-x86-64-linux-gnu_4%3a14.1.0-2ubuntu1_amd64.deb …
Распаковывается g++-x86-64-linux-gnu (4:14.1.0-2ubuntu1) …
Выбор ранее не выбранного пакета g++.
Подготовка к распаковке …/g++_4%3a14.1.0-2ubuntu1_amd64.deb …
Распаковывается g++ (4:14.1.0-2ubuntu1) …
Настраивается пакет libstdc++-14-dev:amd64 (14.2.0-4ubuntu2) …
Настраивается пакет g++-14-x86-64-linux-gnu (14.2.0-4ubuntu2) …
Настраивается пакет g++-x86-64-linux-gnu (4:14.1.0-2ubuntu1) …
Настраивается пакет g++-14 (14.2.0-4ubuntu2) …
Настраивается пакет g++ (4:14.1.0-2ubuntu1) …
update-alternatives: используется /usr/bin/g++ для предоставления /usr/bin/c++ (
c++) в автоматическом режиме
Обрабатываются триггеры для man-db (2.12.1-3) …
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ -std=c++11 -I./include -c sources/print.cpp
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ls print.o
print.o
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ nm print.o | grep print
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ar rvs print.a print.o
ar: создаётся print.a
a - print.o
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ file print.a
print.a: current ar archive
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ -std=c++11 -I./include -c examples/example1.cpp
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ls example1.o
example1.o
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ example1.o print.a -o example1
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ./example1 && echo
hello
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ -std=c++11 -I./include -c examples/example2.cpp
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ nm example2.o
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ g++ example2.o print.a -o example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ./example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat log.txt && echo
hello
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf example1.o example2.o print.o
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf print.a
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf example1 example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf log.txt
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat > CMakeLists.txt <<EOF
> set(CMAKE_CXX_STANDARD 11)
> set(CMAKE_CXX_STANDARD_REQUIRED ON)
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> add_library(print STATIC \${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> include_directories(\${CMAKE_CURRENT_SOURCE_DIR}/include)
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake -H. -B_build
CMake Warning (dev) in CMakeLists.txt:
  No project() command is present.  The top-level CMakeLists.txt file must
  contain a literal, direct call to the project() command.  Add a line of
  code such as

    project(ProjectName)

  near the top of the file, but after cmake_minimum_required().

  CMake is pretending there is a "project(Project)" command on the first
  line.
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) in CMakeLists.txt:
  cmake_minimum_required() should be called prior to this top-level project()
  call.  Please see the cmake-commands(7) manual for usage documentation of
  both commands.
This warning is for project developers.  Use -Wno-dev to suppress it.

-- The C compiler identification is GNU 14.2.0
-- The CXX compiler identification is GNU 14.2.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CMake Warning (dev) in CMakeLists.txt:
  No cmake_minimum_required command is present.  A line of code such as

    cmake_minimum_required(VERSION 3.30)

  should be added at the top of the file.  The version specified may be lower
  if you wish to support older CMake versions for this project.  For more
  information run "cmake --help-policy CMP0000".
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Configuring done (0.5s)
-- Generating done (0.0s)
-- Build files have been written to: /home/luka/Joker762-rgb/workspace/projects/lab03/_build
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build
[ 50%] Building CXX object CMakeFiles/print.dir/sources/print.o
[100%] Linking CXX static library libprint.a
[100%] Built target print
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> add_executable(example1 \${CMAKE_CURRENT_SOURCE_DIR}/examples/example1.cpp)
> add_executable(example2 \${CMAKE_CURRENT_SOURCE_DIR}/examples/example2.cpp)
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> target_link_libraries(example1 print)
> target_link_libraries(example2 print)
> EOF
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build
CMake Warning (dev) in CMakeLists.txt:
  No project() command is present.  The top-level CMakeLists.txt file must
  contain a literal, direct call to the project() command.  Add a line of
  code such as

    project(ProjectName)

  near the top of the file, but after cmake_minimum_required().

  CMake is pretending there is a "project(Project)" command on the first
  line.
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) in CMakeLists.txt:
  cmake_minimum_required() should be called prior to this top-level project()
  call.  Please see the cmake-commands(7) manual for usage documentation of
  both commands.
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) in CMakeLists.txt:
  No cmake_minimum_required command is present.  A line of code such as

    cmake_minimum_required(VERSION 3.30)

  should be added at the top of the file.  The version specified may be lower
  if you wish to support older CMake versions for this project.  For more
  information run "cmake --help-policy CMP0000".
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Configuring done (0.0s)
-- Generating done (0.0s)
-- Build files have been written to: /home/luka/Joker762-rgb/workspace/projects/lab03/_build
[ 33%] Built target print
[ 50%] Building CXX object CMakeFiles/example1.dir/examples/example1.o
[ 66%] Linking CXX executable example1
[ 66%] Built target example1
[ 83%] Building CXX object CMakeFiles/example2.dir/examples/example2.o
[100%] Linking CXX executable example2
[100%] Built target example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build --target print
[100%] Built target print
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build --target example1
[ 50%] Built target print
[100%] Built target example1
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build --target example2
[ 50%] Built target print
[100%] Built target example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ ls -la _build/libprint.a
-rw-rw-r-- 1 luka luka 2238 мар  9 16:09 _build/libprint.a
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ _build/example1 && echo
hello
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ _build/example2
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat log.txt && echo
hello
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf log.txt
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git clone https://github.com/Joker762-rgb/lab03 tmp
Клонирование в «tmp»...
remote: Enumerating objects: 33, done.
remote: Counting objects: 100% (33/33), done.
remote: Compressing objects: 100% (27/27), done.
Получение объектов: 100% (33/33), 11.80 КиБ | 232.00 КиБ/с, готово.
Определение изменений: 100% (7/7), готово.
remote: Total 33 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ mv -f tmp/CMakeLists.txt
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ rm -rf tmp
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cat CMakeLists.txt
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_library(print STATIC ${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_executable(example1 ${CMAKE_CURRENT_SOURCE_DIR}/examples/example1.cpp)
add_executable(example2 ${CMAKE_CURRENT_SOURCE_DIR}/examples/example2.cpp)
target_link_libraries(example1 print)
target_link_libraries(example2 print)
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
CMake Warning (dev) in CMakeLists.txt:
  No project() command is present.  The top-level CMakeLists.txt file must
  contain a literal, direct call to the project() command.  Add a line of
  code such as

    project(ProjectName)

  near the top of the file, but after cmake_minimum_required().

  CMake is pretending there is a "project(Project)" command on the first
  line.
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) in CMakeLists.txt:
  cmake_minimum_required() should be called prior to this top-level project()
  call.  Please see the cmake-commands(7) manual for usage documentation of
  both commands.
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) in CMakeLists.txt:
  No cmake_minimum_required command is present.  A line of code such as

    cmake_minimum_required(VERSION 3.30)

  should be added at the top of the file.  The version specified may be lower
  if you wish to support older CMake versions for this project.  For more
  information run "cmake --help-policy CMP0000".
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Configuring done (0.0s)
-- Generating done (0.0s)
-- Build files have been written to: /home/luka/Joker762-rgb/workspace/projects/lab03/_build
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ cmake --build _build --target install
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ tree _install
Команда «tree» не найдена, но может быть установлена с помощью:
sudo snap install tree  # version 2.1.3+pkg-5852, or
sudo apt  install tree  # version 2.1.1-2ubuntu3
См. 'snap info tree', чтобы посмотреть дополнительные версии.
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ sudo apt install tree
[sudo] пароль для luka: 
                                                                                                                                    К установке:      
  tree

Сводка:
  К обновлению: 0, К установке: 1 К удалению: 0, Не обновляется: 133
  Размер загрузки: 47,1 kB
  Места необходимо: 111 kB / 13,3 GB доступно

Пол:1 http://ru.archive.ubuntu.com/ubuntu oracular/universe amd64 tree amd64 2.1.1-2ubuntu3 [47,1 kB]
Получено 47,1 kB за 0с (514 kB/s)
Выбор ранее не выбранного пакета tree.
(Чтение базы данных … на данный момент устан
овлено 159508 файлов и каталогов.)
Подготовка к распаковке …/tree_2.1.1-2ubuntu
3_amd64.deb …
Распаковывается tree (2.1.1-2ubuntu3) …
Настраивается пакет tree (2.1.1-2ubuntu3) …
Обрабатываются триггеры для man-db (2.12.1-3
) …
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ tree _install
_install  [error opening dir]

0 directories, 0 files
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git add CMakeLists.txt
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git commit -m"added CMakeLists.txt"
[master 16afaf6] added CMakeLists.txt
 1 file changed, 9 insertions(+)
 create mode 100644 CMakeLists.txt
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ git push origin master
Username for 'https://github.com': Joker762-rgb
Password for 'https://Joker762-rgb@github.com': 
Перечисление объектов: 10, готово.
Подсчет объектов: 100% (10/10), готово.
При сжатии изменений используется до 12 потоков
Сжатие объектов: 100% (7/7), готово.
Запись объектов: 100% (9/9), 762 байтов | 762.00 КиБ/с, готово.
Всего 9 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
To https://github.com/Joker762-rgb/lab03.git
   26f9b86..773b80c  master -> master
luka@luka-VirtualBox:~/Joker762-rgb/workspace/projects/lab03$ 
