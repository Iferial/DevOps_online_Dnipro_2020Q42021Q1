Task 8.1


Screenshot 1.


	Я создал два инстанса AWS Linux, поставил на них Apache.
![00.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/00.png)


Screenshot 2.


	Создал в директории /var/www/html пустую HTML страничку. Сложность с которой я столкнулся завлючается в правах моего HTML файла, если владелец файла отличается от владельца, указанного в Jenkins, то job выдаст ошибку [Permission denied], это я понял спустя 20 билдов). На скрине показана смена владельца файла.
![01.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/01.png)


Screenshot 3.


	Далее я содал два job, один для тестового сервера, другой для production. 
![02.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/02.png)


Screenshot 4.


	В конфиге джоба у меня создаётся HTML страничка со ссылками на мой AWS прогресс.
![03.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/03.png)


Screenshot 5.


	С помощью плагина Publish over SSH устанавливаю коннект с моими серверами в AWS и даю доступ к директории с HTML файлом.
![04.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/04.png)


Screenshot 6.


	Так выглядит настройка для плагина в джобе. Я заменяю .html файл на созданный мной и перезагружаю Apache командой sudo service httpd restart.
![05.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/05.png)


Screenshot 7.


	Успешный Deploy и вывод в консоли.
![06.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/06.png)


Screenshot 8.


	 И полученные изменения на нашем тетовом сервере и в последствии и на production сервере.
![07.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m8/task8.1/screenshots/07.png)




