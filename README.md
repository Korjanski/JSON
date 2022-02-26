# JSON
1. Создать внешний репозиторий c названием JSON.
зайти на сайт https://github.com
войти под своей учетной записью
нажать на вкладку Repositories
нажать на зеленую кнопку NEW
в поле Repository name ввести JSON
выбрать  Public
поставиь галочку Add a README file
нажать create repository

 2. Клонировать репозиторий JSON на локальный компьютер.
нажать Code выбрать пункт Https
далее скопировать ссылку,зайти в папку,куда будет скопирован репозиторий
git clone https://github.com/Korjanski/JSON.git

 3. Внутри локального JSON создать файл “new.json”.
git touch new.json
git status файл new.json не отслеживается(горит красным)

 4. Добавить файл под гит.
git add new.json (добавляем файл под гит)
git status new.json отслеживается(горит зеленым)

 5. Закоммитить файл.
git commit -m "add new.json"

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
vim new.json
i

{
		"name":"Dergachev Sergey",
		"age":34,
		"home pets":"no",
		"future desire salary":"700$"
}
esc
:wq
 8. Отправить изменения на внешний репозиторий.

git commit -am "changed new.json"
git push

 9. Создать файл preferences.json
touch preference.json

 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
vim prefenrence.json
i
{	"favorite movie":"pulp fiction",
	"favorite serial":"brassic",
	"favorite food":"sushi",
	"favorite time of the year":"summer",
	"country i would like to visit":"Great Britain"
}

esc
:wq
 
11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
cat>skills.json
{"skills":["json","xml","txt","github","gitbash"]}

Enter
Ctrl+D
 12. Отправить сразу 2 файла на внешний репозиторий.
git add .;git commit -m"add skills.json,preference.json";git push


 13. На веб интерфейсе создать файл bug_report.json.
нажать add file
выбрать create new file
в поле name new file ввести bug_report.json

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
нажать кнопку commit new file

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
открыть файл bug_report.json
{"hello Kitty"}

 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
нажать commit change

 17. Синхронизировать внешний и локальный репозиторий JSON
git pull ввести в терминале
