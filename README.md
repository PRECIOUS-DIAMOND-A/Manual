# Manual

1. Показать все ветки:
   git branch
   
2. Переключение между ветвями:
   git checkout <название_ветки>  # или git switch <название_ветки>, если используется Git версии 2.23 и выше
   
3. Создание ветвей:
   git branch <название_ветки>
   
4. Удаление ветвей:
   git branch -d <название_ветки>  # Для безопасного удаления (проверяет, были ли внесены изменения)
   git branch -D <название_ветки>  # Для принудительного удаления (не проверяет изменения)
   
5. Слияние ветвей:
   Сначала переключитесь на ветку, в которую вы хотите слить изменения, а затем выполните:
   git merge <название_ветки>
   


1. Переключитесь на ветку `master` в своем локальном репозитории:
       git checkout master
    
2. Сливайте изменения из ветки `main` с веткой `master`:
       git merge main
    
3. Отправьте изменения в удаленный репозиторий на GitHub:
       git push origin master



Чтобы ваш локальный репозиторий узнал о существовании ветки main на удаленном репозитории GitHub, вам нужно выполнить следующую команду:
git fetch origin main:main



Для отправки файлов в репозиторий:
git add <имя_файла>
git commit -m "Ваше сообщение коммита"
git push


Для загрузки файлов из репозитория:
git pull


Для глобальной отправки изменений файлов в репозиторий:
git add .
git commit -m "Ваше сообщение коммита"
git push

Вход в свой аккаунт GitHub:
git config --global user.name "My Name"
git config --global user.email myEmail@example.com

Клонирование репозитория (если репозиторий уже существует):
git clone <ссылка_на_репозиторий>
cd <название_репозитория>

Инициализация нового репозитория (если репозиторий еще не существует):
git init

Добавление файлов в индекс:
git add <имя_файла>

Фиксация изменений:
git commit -m "Ваше сообщение коммита"

Связывание локального репозитория с удаленным на GitHub:
git remote add origin <ссылка_на_репозиторий>

Отправка изменений в репозиторий на GitHub:
git push -u origin master

Отправка изменений в основную ветку:
git add .
git commit -m "Ваше сообщение коммита"
git push origin main

Создание новой ветки, переключение на неё и отправка изменений:
git branch <название_ветки>
git checkout <название_ветки>  # или git switch <название_ветки>, если используется Git версии 2.23 и выше
git add .
git commit -m "Ваше сообщение коммита"
git push origin <название_ветки>

