# Урок 2. Итоговая контрольная работа

## Информация о проекте:

Организуйте систему учёта для питомника, в котором живут домашние и вьючные животные.

# Задание с решением
1) Используя команду cat в терминале операционной системы Linux, создать
два файла Домашние животные (заполнив файл собаками, кошками,
хомяками) и Вьючные животными заполнив файл Лошадьми, верблюдами и
ослы), а затем объединить их. 

    $ cat > pets.txt
   
    $ cat > pack_animals.txt
   
    $ cat pets.txt pack_animals.txt > all_animals.txt

<img width="934" height="295" alt="1 (1)" src="https://github.com/user-attachments/assets/b07976cb-b552-4e9a-b79e-2e02cf16d893" />

Просмотреть содержимое созданного файла. Переименовать файл, дав ему новое имя (Друзья человека).

    $ cat all_animals.txt
    
    $ mv all_animals.txt human_friends.txt

<img width="934" height="437" alt="1_2" src="https://github.com/user-attachments/assets/ba35fc02-3203-4458-a189-693c718ab74e" />


2) Создать директорию, переместить файл туда.

    $ mkdir animal
   
    $ mv human_friends.txt animal/

<img width="934" height="307" alt="2 (1)" src="https://github.com/user-attachments/assets/af3650db-7719-47d2-8e2c-5c0f9e3538eb" />

3) Подключить дополнительный репозиторий MySQL. Установить любой пакет
из этого репозитория.

    $ sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
   
    $ sudo apt update

4) Установить и удалить deb-пакет с помощью dpkg.

   $ sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
   
   $ sudo dpkg -r mysql-apt-config
   
   $ sudo dpkg --purge mysql-apt-config
   

5) Нарисовать диаграмму, в которой есть класс родительский класс, домашние
животные и вьючные животные, в составы которых в случае домашних
животных войдут классы: собаки, кошки, хомяки, а в класс вьючные животные
войдут: Лошади, верблюды и ослы).

<img width="981" height="578" alt="image" src="https://github.com/user-attachments/assets/b341f0e9-1f81-43b8-963c-d091d4aff2a4" />

<img width="1036" height="584" alt="image" src="https://github.com/user-attachments/assets/70bd5da9-750b-42fd-87fd-1bc5cb582dd0" />


6) В подключенном MySQL репозитории создать базу данных “Друзья
человека”

   CREATE DATABASE IF NOT EXISTS HumanFriends;
   
   USE HumanFriends;
   
7) Создать таблицы с иерархией из диаграммы в БД

<img width="935" height="814" alt="1 1" src="https://github.com/user-attachments/assets/d073d429-af98-40f7-980c-bbf1d2398570" />
<img width="904" height="288" alt="2 2" src="https://github.com/user-attachments/assets/984d18ca-ae2c-4593-a321-c15df617e820" />




8) Заполнить низкоуровневые таблицы именами(животных), командами
которые они выполняют и датами рождения


<img width="940" height="819" alt="1 3" src="https://github.com/user-attachments/assets/b69b102b-7536-4115-bac6-ddfb490485bb" />
<img width="902" height="153" alt="1 4" src="https://github.com/user-attachments/assets/150a85cd-cedc-4998-94ed-cb2f406dcc32" />


9) Удалив из таблицы верблюдов, т.к. верблюдов решили перевезти в другой
питомник на зимовку. Объединить таблицы лошади, и ослы в одну таблицу.


<img width="922" height="210" alt="1 1" src="https://github.com/user-attachments/assets/c9e8f4ae-0b52-41a9-b115-d6c917864d54" />


10) Создать новую таблицу “молодые животные” в которую попадут все
животные старше 1 года, но младше 3 лет и в отдельном столбце с точностью
до месяца подсчитать возраст животных в новой таблице


<img width="937" height="180" alt="2025-08-05_11-38-01" src="https://github.com/user-attachments/assets/96255594-0215-409c-b343-913e099550b2" />


11) Объединить все таблицы в одну, при этом сохраняя поля, указывающие на
прошлую принадлежность к старым таблицам.


<img width="937" height="104" alt="2025-08-05_11-38-34" src="https://github.com/user-attachments/assets/ff54df32-7a15-4a75-98ef-aa8c69b3cf06" />


