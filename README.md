# PP_nagletsi_iz_matritsi_125
Здравствуйте, уважаемые организаторы соревнований!
Сейчас мы активно заняты разработкой самого приложения и корректировкой формы данных для базы данных, поэтому времени составлять подробные(любые) DFD и UML диаграммы нет.

Архитектура

Пока, можем только перечислить модули, точнее, разделы.
Грубо говоря, три раздела: спортсмен, организатор, платформа.

Всё, что касается связи с БД, отправки запросов, получения ответов, сохранения информации, вывода информации на платформу (новости, соревнования, заявки и т.д.) будут определены в разделе "платформа", разумеется, с разбивкой на модули.
В разделах "спортсемен" и "организатор" будут определены функции формирования команды, подачи заявки, одобрения/отклонения заявок, само формирование заявки, обработка, сохранение и т.п., будут также реализованы в разделе "платформа".

Итого: один большой раздел "платформа" и два маленьких.

P.S. Скорее всего появится ещё подраздел раздела "платформа" - раздел "соревнования", в котором будет хранится вся настоящая информация о проводимых соревнованиях.

ER-диаграмма БД была где-то на листочке, потерялась)

В принципе, не важно, так как сама база данных уже написана.

Что касается базы данных, выбрали мы PostgreSQL.
Почему?

Причина 1:
![image](https://github.com/user-attachments/assets/580dbf24-cc47-499a-943c-0966a85e2458)

Причина 2: Она развернётся, практически, на любой ОС, что, по сути, делает её кроссплатформенной для сервера)
