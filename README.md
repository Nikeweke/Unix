## Unix(Ubuntu)

### Packages(Ubuntu - apt-get)
* **sudo apt-get install pkg_name** - установка пакета
* **sudo apt-get remove pkg_name** - удаление пакета
* **sudo apt-get install nano** - текстовий редактор который откроет файл в консоли(**Ctrl+W - search, Ctrl+X - save**)

### Commands
* **sudo su** - получени прав root
* **killall name_proccess** - убить процесс
* **top** - действующие процессы
* **uptime** - сколько в работе 
* **sudo apt-get update** - обновить установщик
* **ls -A** - показать все файлы в текущей директории (**-А** - включая скрытые)
* **cd /path/to/dir/** - перейти в директорию
* **cd ..** - спуститься на 1 папку вниз
* **sudo mkdir nameOfDir** - сделать папку 
* **sudo atom index.php** - открыть файл с помощью Атома, если такого файла нет -то создаст
* **sudo rm filename** - удалить файл
* **sudo rm directory -r** -  удалить папку
* **(cd /path/to/filename) sudo chmod +x filename.sh** - сделать файл допустимым для запуска
* **./filename** - запуск файла(без разширения)
* **bash filename.sh** - запуск с разширением
* **dpkg -s filename** - установлен ли пакет ?
* **whereis filename** - где пакет
* **du -hs /path/to/directory** - вес папки

### Launching files
* Launch file without **.sh** - `./filename`
* Launch **file.sh** - `bash filename.sh`

### Права на папку и переименование
* **sudo chmod -R a+wx folder** - все права на папку для исполнения там действий
* **sudo mv robot robot_new** - переименовать папку
* `HELP commands  when HOLD windows button

### Node JS Deploy решение почему же приложение падает после закрытия окна
Запуск был такой : `node app prod &`; Все работает отлично когда Putty окно открыто, после падает приложение. В чем проблема была? Был вывод в приложении `console.log` и надо либо убрать этот вывод либо писать в файл лог вот так:
```
# Запись вывода приложения в файлик
$ node app prod & >> log.txt
```

### Удаление Nginx под чистую 
```
apt-get remove --purge nginx nginx-full nginx-common
apt-get install nginx
```


### Deploying Laravel on VPS, LEMP(Linux, Nginx, MySQL, PHP)
http://devmarketer.io/learn/deploy-laravel-5-app-lemp-stack-ubuntu-nginx/

