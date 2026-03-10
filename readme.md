#Задача Терминал(пользователи) Роман Салий

1.
   -Создал пользователя vally с оболочкой useradd -m -s.

   -Создал пользователя eve без каталога домашнего useradd.

   -Создал директорию /home/eve и дал права eve chown eve:eve /home/eve.



2.
   -Проверил id vally.

   -Изменил имя vally на robot usermod -l.

   -Создал группу tms groupadd.

   -Добавил robot в группу tms usermod -aG.
   
   -Скриншот 3 относится к пункту 2.



4.
   -Создал директорию /var/www/projetcs.

   -Файлы readme.md, secret, bot-hub/app.py.



5.
   -chmod 600 для файла secret(только владелец).

   -chmod g+rw для файла readme(группа и владелец).

   -chmod 666 для bot-hub/app.py(убрал бит x у всех).

   -chomd ug+x для bot-hub/app.py(возврат бита x).



6.
   -Рекурсивно назначил владельца /var/www/projects группу tms командой chgrp -R.

   -Назначил владельца secret пользователя robot. 

   -Назначил владельца readme.md пользователя eve.

   -Для назначения использовал chown.
