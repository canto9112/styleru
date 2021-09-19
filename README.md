# Рекомендации фильмов с сайта - [themoviedb.org](https://www.themoviedb.org/)

Скрипт рекомендует фильмы которые были добавлены в базу данных

### Как установить

У вас уже должен быть установлен Python 3. Если его нет, то установите.
Так же нужно установить необходимые пакеты:
```
pip3 install -r requirements.txt
```


### Получение API ключа

1. Зарегистрироваться на сайте - [TMDB](https://www.themoviedb.org/);
2. Создать приложение - выбрать [Developer](https://www.themoviedb.org/settings/api/request);
3. Перейти на страницу [API](https://www.themoviedb.org/settings/api) и получчить API ключ;


### Получение базы с фильмами

1. Запустить файл make_own_db.py командой:
```
python make_own_db.py
```
2. Скрипт запросит у вас API ключ. Вставьте свой ключ после фразы и нажмите Enter:

```
Enter your api key v3:71941b5d49d6d1721eecbf079a161647
```
3. После нажатия Enter в консоли будут выводиться прогресс скачивания фильмов.
   Это может занять 10-15 минут, нужно подождать. После завершения у вас появиться файл с именем:
   ```MyFilmDB.json```
   

### Получение рекомендаций

1. Запустить файл find_similar.py командой:
```
python find_similar.py
```
2. Скрипт попросит ввести имя файла с базой данных фильмов. Вставьте ```MyFilmDB.json``` и нажмите Enter:

```
Enter path to DataBase:MyFilmDB.json
```
3. После того как скрипт проверит все-ли в порядки с вашим файлом он попросит ввести название фильма:

```
Enter film to search for:Ariel
```
Название фильма нужно вводить на Английском языке!

4. Результат:
```
Enter path to DataBase:MyFilmDB.json
Enter film to search for:Ariel
========================
Elsker dig for evigt
Hable con ella
Kunstgriff
Las Hurdes
Megacities
My Life Without Me
Sonntag im August
The Dark
Varjoja paratiisissa
```





