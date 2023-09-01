# ***Работа с удалёнными репозиториями***
1. Создать аккаунт на GitHUb.
Для работы с удалённым репозиторием необходимо создать аккаунт на GitHub`е. Нужно ввести свою электронную почту, а затем придумать пароль для своего аккаунта.

2. Создать удалённый репозиторий.
На странице профиля в GitHub необходимо создать удалённый репозиторий с помощью значка "+". Откроется страница под названием `Create a new repository`. Вводим имя для нашего ***удалённого*** репозитория, после создаём наш репозиторий с помощью кнопки `Create repository` (кнопка зелёного цвета).
Затем GitHub  предложит 3 варианта действий для создания репозитория.

а. Создать локальный репозиторий, при условии, если у нас нет локального репозитория. ( Проводится стандартная операция по созданию локального репозитоия с помощью базовых команд `git init`, `git add <file>`, `git commit -m` и так далее...)

б. Связывание локального репозитория с удалённым. 
Первая команда `git remote add origin (адресс нашего удалённого репозитория)` связывает локальный репозиторий с удалённым.
Вторая команда `git branch -M main` переименовывает нашу ветку в основную - ***main***
Третья команда `git -u origin main` отправляет изменения в 
удалённый репзиторий. 

в. Отправка кода с другого репозитория. 
`import code`

3. Создать локальный репозиторий.
Для создания локального репозитория необходимо сначала создать папку, а после в ней инициализировать  репозиторий с помощью команды `git init`.

4. Связать удалённый репозиторий с локальным.

Добавление удалённого репозитория к локальному происходит засчёт команды `git remote add <имя репозитория><url-адрес репозитория в сети>`
Также после можно проверить, связался ли удалённый репозиторий с локальным с помощью команды `git remote`. После этой команды при правильном алгоритме действий в терминале должно вылезти сокращённое название удалённого репозитория `origin`.

Чтобы ветки локального и удалённого репозитория не путались, не будет лишним переименовать основную ветку локального репозитория также, как переименовывали ветку у удалённого репозитория с помощью команды `git branch -M main`.

Отправить изменения локального репозитория в удалённый `git push`.
Для получения и слияния изменений с удалённого реепозитория используется команда: `git pull`.

