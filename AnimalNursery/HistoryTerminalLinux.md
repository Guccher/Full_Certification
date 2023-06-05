## 1. Используя команду cat в терминале операционной системы Linux, создать два файла Домашние животные (заполнив файл собаками, кошками, хомяками) и Вьючные животными (заполнив файл Лошадьми, верблюдами и ослы), а затем объединить их. Просмотреть содержимое созданного файла. Переименовать файл, дав ему новое имя (Друзья человека).

    guccher@simon-Ubuntu:~$ cat > home_animals
    dogs
    cats
    hamsters
    guccher@simon-Ubuntu:~$ cat > pack_animals
    horses
    camels
    donkeys
    guccher@simon-Ubuntu:~$ cat home_animals pack_animals > animals
    guccher@simon-Ubuntu:~$ cat animals
    dogs
    cats
    hamsters
    horses
    camels
    donkeys
    guccher@simon-Ubuntu:~$ mv animals mans_friends
    guccher@simon-Ubuntu:~$ 1s -ali

## 2. Создать директорию, переместить файл туда.

    guccher@simon-Ubuntu:~$ mkdir nursery
    guccher@simon-Ubuntu:~$ cd nursery/
    guccher@simon—Ubuntu:~/nursery$ pwd
    /home/guccher/nursery
    guccher@simon-Ubuntu:~/nursery$ cd ..
    guccher@simon-Ubuntu:~$ mv mans_friends /home/guccher/nursery
    guccher@simon-Ubuntu:~$ cd nursery/
    guccher@simon-Ubuntu:~/nursery$ 1s
    nans_friends

## 3. Подключить дополнительный репозиторий MySQL. Установить любой пакет из этого репозитория. 

    guccher@simon-Ubuntu:~/nursery$ sudo wget https: //dev.mysql.com/get/mysql-apt-config_@.8.23-1_all.deb

    guccher@simon-Ubuntu:~/nursery$ sudo dpkg -i mysql-apt-config_®.8.23-1_all.deb

    guccher@simon-Ubuntu:~/nursery$ sudo apt-get update

    guccher@simon—-Ubuntu:~/nursery$ sudo apt-get install mysql-server
## 4. Установить и удалить deb-пакет с помощью dpkg.

    sudo wget https://download.docker.com/linux/ubuntu/dists/jammy/pool/stable/amd64/docker-ce-cli_20.10.13~3-0~ubuntu-jammy_amd64.deb

    sudo dpkg -i docker-ce-cli_20.10.133-0ubuntu-jammy_amd64.deb

    sudo dpkg -r docker-ce