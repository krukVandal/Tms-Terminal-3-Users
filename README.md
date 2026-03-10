#Задача Терминал(пользователи) Роман Салий

1.
   -Создал пользователя vally с оболочкой useradd -m -s.

   -Создал пользователя eve без каталога домашнего useradd.

   -Создал директорию /home/eve и дал права eve chown eve:eve /home/eve.

<img width="642" height="227" alt="image" src="https://github.com/user-attachments/assets/b8d84b88-42c5-447c-8ab4-5d9a7b506b27" />


2.
   -Проверил id vally.

   -Изменил имя vally на robot usermod -l.

   -Создал группу tms groupadd.

   -Добавил robot в группу tms usermod -aG.
 
   -Скриншот 3 относится к пункту 2.

<img width="1226" height="443" alt="image" src="https://github.com/user-attachments/assets/f3c1db8b-7af7-4d55-a435-69cf9bdf3bbe" />

<img width="1226" height="659" alt="image" src="https://github.com/user-attachments/assets/a82f1a22-392d-4041-8c2e-3f43904c68a6" />


4.
   -Создал директорию /var/www/projetcs.

   -Файлы readme.md, secret, bot-hub/app.py.

<img width="706" height="533" alt="image" src="https://github.com/user-attachments/assets/80bab174-1c63-464e-9689-fd19300da283" />


5.
   -chmod 600 для файла secret(только владелец).

   -chmod g+rw для файла readme(группа и владелец).

   -chmod 666 для bot-hub/app.py(убрал бит x у всех).

   -chomd ug+x для bot-hub/app.py(возврат бита x).

<img width="1162" height="803" alt="image" src="https://github.com/user-attachments/assets/bc00d192-a537-463d-9735-8990f134c1d9" />


6.
   -Рекурсивно назначил владельца /var/www/projects группу tms командой chgrp -R.

   -Назначил владельца secret пользователя robot. 

   -Назначил владельца readme.md пользователя eve.

   -Для назначения использовал chown.

<img width="938" height="677" alt="image" src="https://github.com/user-attachments/assets/d69fa03a-38bc-492d-8ff2-a9011014fd9e" />

