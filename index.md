Задания выполненые на курсе по темам:
BASH
https://github.com/lozaim/dockerhw
-Создал который получает на вход параметр (имя пользователя), по нему определятся путь.После вызывается функция которая проверяет доступность указанных папок, если папок нет, создает их, и копирует файли из папки SRC в папку DST. Пути папок хранятся в переменных и локально.

Docker
https://github.com/lozaim/dockerhw
-Через docker поднял тремя способами mysql базу с phpmyadmin
-Через docker-compose поднял MySQL базу с двумя wordpress сайтами nginx и phpmyadmin, файлы настроек и база хранятся локально

AWS
https://github.com/lozaim/awshw
-Создал с помощью AWS CLI и CloudFormation, отказоустойчивую VPC в двух Availability zones с database subnet (без выхода в интернет) private subnet (с выходом в интернет через nat gateway) и public subnet (с выходом в интернет через internet gateway)
-Создал EC2 instance с помощью AWS CLI и CloudFormation. Во время создания instance с s3 bucket копируется скрипт который устанавливает httpd, и создается страница со списком подсетей VPC
-Создал ASG через CloudFormation подключенную к VPC
-Создал с помощью packer образ в котором запущен веб сервер, и создана страница с именем ОС данного образа и датой его создания
-С помощью cloudformation создал EC2 с образом созданым в п.1
-С помощью cloudformation создал SNS topic и subscription с моим email. Email передаеться параметром.
-Создал s3 бакет и настроил уведомления на email при созании/удалении объекта в бакете

Jenkins
https://github.com/lozaim/aws-jenkins
-Создал параметризированный Jenkins Job, который выкачивает из GitHub CloudFormation template и подставляет в него параметры из Jenkins Job
-Создал виртуальную машину в AWS используя Jenkins Job, после ее создания ее ID передается Jenkins console output
