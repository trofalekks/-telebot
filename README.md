# -telebot
Это словарь по telebot
Он будет постепенно пополняться



Обязательные строки:
bot = telebot.TeleBot('Токен') - токен от бота
bot.polling() - в конце бота запускается функция проверки новых сообщений
@bot.message_handler(commands=['start']) Цикл который запускается при команде старт

Контент:
@bot.message_handler(content_types=['text'])
@bot.message_handler(content_types=['sticker'])
это типо пример записи.

Все виды контента:
ONTENT_TYPES = ["text", "audio", "document", "photo", "sticker", "video", "video_note", "voice", "location", "contact", "new_chat_members", "left_chat_member", "new_chat_title", "new_chat_photo", "delete_chat_photo","group_chat_created", "supergroup_chat_created", "channel_chat_created", "migrate_to_chat_id", "migrate_from_chat_id", "pinned_message"]

Ответы на команды(примеры записи):
@bot.message_handler(commands=['текст команды'])
и после писать что хочешь.

Отправка сообщения:
bot.send_message-(вид контента)(message.chat.id, "праанглопапропро")
Отправка стикера:
bot.send_sticker(message.chat.id, 'CAADAgADZgkAAnlc4gmfCor5YbYYRAI') по id 

Реакция на сообщение:
if message.text.lower() == 'привет'

Клавиатура:
Вызов клавиатуры
keyboard1 = telebot.types.ReplyKeyboardMarkup()
