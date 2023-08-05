## Покрытие тестами проекта «Yatube»
### Реализовано
- тестирование модели приложения posts в Yatube;
- проверка доступности страниц и названия шаблонов приложения Posts проекта Yatube, проверка учитывает права доступа;
- проверка корректности использования html-шаблонов во view-функциях;
- проверка соответствия ожиданиям словаря context, передаваемого в шаблон при вызове;
- проверка на корректное отображение поста на главной странице сайта, на странице выбранной группы и в профайле пользователя при создании поста и указании группы, а также проверка, что пост не попал в группу, для которой не был предназначен;
- проверка создания новой записи в базе данных при отправке валидной формы со страницы создания поста, а при отправке валидной формы со страницы редактирования поста изменение поста с post_id в базе данных.

### Как запустить проект:
* Клонировать репозиторий и перейти в него в командной строке: 
  ```
  git clone https://github.com/pavelboykov/hw04_tests.git
  cd hw04_tests
  ```
* Cоздать и активировать виртуальное окружение:
  * Windows
     ```
     python -m venv env
     source venv/Scripts/activate
     ```
  * Linux
    ```
    python3 -m venv venv
    source venv/bin/activate
    ```
* Установить зависимости из файла requirements.txt:
  * Windows
    ```
    python -m pip install --upgrade pip
    pip install -r requirements.txt
    ```
  * Linux
    ```
    python3 -m pip install --upgrade pip
    pip install -r requirements.txt
    ```
* Выполнить миграции:
  * Windows: 
    ```
    python manage.py migrate
    ```
  * Linux: 
    ```
    python3 manage.py migrate
    ```
* Запустить проект:
  * Windows: 
    ```
    python manage.py runserver
    ```
  * Linux: 
    ```
    python3 manage.py runserver
    ```
