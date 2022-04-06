# async_tg_bot
##Tg-bot that gives you recipes at your request. Written using aiogram and postgresql database

###Установка
Для корректной работы необходимо установить все модули из файла *requirements.txt*. Для этого введите у себя в консоли:
```
$ pip3 install -r requirements.txt
```

### Запуск
Для хранения персональных переменных, таких как токен бота и учётные данные базы postgres я использовал возможности модуля `python-dotenv`.
Если вы хотите Запустить программу со своими данными, создайте в основной директории файл *.env* и положите в него следующие переменные:
```
TG_BOT_TOKEN = 'Ваши данные'
DB_LOGIN = 'Ваши данные'
DB_PASSWORD = 'Ваши данные'
DB_NAME = 'Ваши данные'
```
Для создания таблицы в БД запустите отдельно файл *tg_bot_app/models.py*. 
Далее для заполнения таблицы вашими рецептами воспользуйтесь скриптом *tg_bot_app/add_recipe.py*.
И наконец запуск самого бота будет осуществляться через файл *bot.py*. Начинайте общение через команду */start* 
