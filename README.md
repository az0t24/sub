# Инструкция. 

## Выделение отдельного репозитория из папки.

1. Создаем папку, переходим в нее и инициализируем репозиторий.
2. Клонируем себе репозиторий через комбинацию команд: `git remote add origin "https://github.com/meshy/django-schema-graph.git"` и `git pull origin main`
3. Оставляем только интересующую нас папку: `git filter-branch --subdirectory-filter assets -- --all`
4. Подключаем собственный репозиторий: `git remote add my_repo "https://github.com/az0t24/django.git"`
5. И наконец: `git push -u my_repo master`

## Добавление submodule в репозиторий.

1. Добавляем в репозиторий: `git submodule add "https://github.com/az0t24/django.git"`
2. Коммитим и пушим изменения.
