
	Как это работает?

	1. Создаете папку, помещаете в нее тесты, которые хотите прогнать
	2. Запускаете скрипт с помощью  $ ./<script name>
	3. Указываете название папки, в которой лежат файлы для тестирования

По умолчанию каждый раз, когда происходит git commit, система запрашивает ваш пароль. Чтобы избежать этого нужно выполнить следующие команды: 
   Если git подключен с помощью git@github.com:<your username>/<repository name>.git
     $ eval `ssh-agent -s`
     $ ssh-add
   Если git подключен с помощью https://github.com/<your username>/<repository name>.git (но это вряд ли)
     $ git config credential.helper store
     $ git config --global user.name "<your username>"
     $ git config --global user.password "<your password>"
