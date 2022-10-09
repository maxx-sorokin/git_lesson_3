# Инструкция по работе с Git

>Более подробная инструкция по работе с Git для новичков представлена [здесь](https://habr.com/ru/post/541258/ "часть 1") и [здесь](https://habr.com/ru/post/542616/ "часть 2").

## Начало работы

1. ***Скачать и установить*** [*Git*](https://git-scm.com/downloads), **а также** [*Microsoft Visual Studio Code*](https://code.visualstudio.com/Download)
2. После установки необходимо «представиться» системе контроля версий. Это нужно сделать всего один раз, и git запомнит вас. Для этого нужно ввести в терминале 2 команды:
• *git config --global user.name «Ваше имя английскими буквами»*
• *git config --global user.email ваша почта@example.com*

## Основные команды

* *git init* – инициализация локального репозитория
* *git status* – получить информацию от git о его текущем состоянии
* *git add* – добавить файл или файлы к следующему коммиту
* *git commit -m “message”* – создание коммита.
* *git log* – вывод на экран истории всех коммитов с их хеш-кодами
* *git checkout* – переход от одного коммита к другому
* *git checkout master* – вернуться к актуальному состоянию и продолжить работу
* *git diff* – увидеть разницу между текущим файлом и закоммиченным файлом

#### Команды для ветвления

* *git branch* – посмотреть список веток в репозитории
* *git branch <название ветки>* – создать новую ветку
* *git checkout <название ветки>* – переход к другой ветке
* *git branch -d <название ветки>* – удалить ветку

### Примеры использования комманд

На скриншоте ниже можно увидеть последовательность действий для создания нескольких коммитов в файле. Также видно, как были применены команды *git status*, *git log* и *git diff*

![Основные команды](1.jpg)

На следующих двух скриншотах видно, как осуществляется переключение между коммитами.

![Первый коммит](2.jpg)
![Последний коммит](3.jpg)

## Работа с удалённым репозиторием

### Команды

* *git clone <url-адрес репозитория>* – клонирование внешнего репозитория на локальный ПК
* *git pull* – получение изменений и слияние с локальной версией
* *git push* – отправляет локальную версию репозитория на внешний