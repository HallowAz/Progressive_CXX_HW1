# Домашнее задание №1 по курсу "Программирование на современном C++"

## Задание

Необходимо разработать программу, которая обрабатывает данные онлайн сервиса MusicBrainz.

Датасет можно скачать на официальном сайте MusicBrainz https://data.metabrainz.org/pub/musicbrainz/data/fullexport/

Необходимый файл mbdump.tar.bz2.

Описание датасета находится по ссылке https://musicbrainz.org/doc/MusicBrainz_Database/Schema

Например, для Артиста диаграмма находится по ссылке https://wiki.musicbrainz.org/images/7/7e/artist_entity_details.svg

Файл датасета представляет из себя сжатый архив из множества текстовых файлов, где данные располагаются в строчках, а поля разделены символом табуляции \t

Каждая таблица на схемах представлена отдельным файлом с аналогичным названием

Программа должна принимать необходимые для работы имена распакованных файлов в качестве аргументов командной строки и выводить данные в стандартный вывод.

Программа не должна использовать интерактивный ввод с клавиатуры, например, "введите имя файла", "введите необходимый год", "ведите q чтобы выйти" - такими программами не удобно пользоваться и их разработка занимает больше времени.

### Ваш вариант:

Вывести число мужчин и женщин исполнителей, живших в год, который передан в аргументах командной строки

### Решение

Для запуска программы необходимо собрать её с помощью cmake и вызвать make из корневой папки.

 Затем запустить исходник в формате

    ./hw1.exe --artistiFilename=static/test_artist genderFilename=static/test_gender year=*год* 

 Порядок аргументов не важен
