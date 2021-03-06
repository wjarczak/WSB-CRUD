# Choose Your language
## [English](#ENG)
## [Polish](#PL)

# ENG

>I created that code using Visual Studio Code on MacOS with Python 3.10

>Django documentation [docs.djangoproject.com](https://docs.djangoproject.com/en/3.2/)

## About The Project

It's CRUD (Create, Read, Update, Delete) created for Wyższa Szkoła Bankowa in Gdansk.

## Getting Started
I assume that Your knowledge of Python is one that point where you know what is virtual environment, and how to use it.
>Make sure you have installed Python 3 and virtual environment on your device
1. Create virtual environment and activate inside your directory

```
virtualenv env
source env/bin/activate
```
2. Install all dependencies in `requirements.txt` to start work with this project

```
pip install -r requirements.txt
```
3. Every after change `models.py` you need to make migrations into `db.sqlite3` (database) to create the table for the new model

```
python manage.py makemigrations
python manage.py migrate
```

3. If it doesn't create the `students student` or` students representative` table, do migrations with sync

```
python manage.py migrate --run-syncdb
```

4. Create `superuser` and test the project

```
python manage.py createsuperuser
python manage.py runserver
```

5. If you want to add students from `.csv` run command --Currently not working

```
python manage.py runscript load_students
```

## License

Distributed under MIT License.
<!-- CONTRIBUTORS -->
## Code Contributors

This project exists thanks to:\
Wojciech Jarczak - [github.com/wjarczak](https://github.com/wjarczak)

## Project Link
[github.com/wjarczak/WSB-CRUD](https://github.com/wjarczak/WSB-CRUD)

# PL

>Stworzyłem ten kod za pomocą Visual Studio Code na MacOS z Pythonem 3.10

>Dokumentacja django [docs.djangoproject.com](https://docs.djangoproject.com/en/3.2/)

## O projekcie

CRUD (Create, Read, Update, Delete) stworzony dla Wyższej Szkoły Bankowej w Gdańsku.

## Pierwsze kroki

Zakładam, że Twoja znajomość Pythona jest na poziomie, w którym wiesz czym jest środowisko wirtualne i jak z niego korzystać.
>Upewnij się, że zainstalowałeś Python 3 i środowisko wirtualne na swoim urządzeniu
1. Stwórz wirtualne środowisko i aktywuj w swoim katalogu

```
virtualenv env
source env/bin/activate
```
2. Zainstaluj wszystkie zależności z pliku `requirements.txt`, aby rozpocząć pracę projektem

```
pip install -r requirements.txt
```
3. Po każdej zmianie `models.py` należy dokonywać migracji do `db.sqlite3` (baza danych), aby utworzyć tabelę dla nowego modelu

```
python manage.py makemigrations
python manage.py migrate
```

3. Jeżeli nie utworzy tabeli `students_student` lub `students_representative` to wykonaj migracje z synchronizacją

```
python manage.py migrate --run-syncdb
```

4. Utwórz `superuser` i przetestuj projekt

```
python manage.py createsuperuser
python manage.py runserver
```

5. Jezeli chcesz dodac studentów z pliku `.csv` uruchom komendę --Aktualnie nie działa

```
python manage.py runscript load_students
```

## Licencja

Projekt dystrybuowany jest na licencji MIT.

## Twórca kodu

Projekt istnieje dzięki:\
Wojciech Jarczak - [github.com/wjarczak](https://github.com/wjarczak)

## Link do projektu
[github.com/wjarczak/WSB-CRUD](https://github.com/wjarczak/WSB-CRUD)