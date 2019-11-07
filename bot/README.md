# Модули для работы программы.

## CommandHandler

Обработчик команд. Команды вытаскивает из коллекции Map

## CommandLoader

Загрузчик команд. Загружает в коллекцию Map.

Загружает данные:

- name: Название команды.
- ЧС: Чёрный список, то есть ID людей у которых команда не будет работать.
- bot: Можно ли использовать команды ботам?
- DM: Можно ли использовать команды в ЛС?
- owner: Команда будет доступна только создателю или всем?

## DM

Транслирует сообщения из ЛС в специальный канал.

## GuildMemberAdd

Делает действие при входе пользователя.

- Приветствует его на сервере или в лс.

Если бота не настраивали на сервере то ничего не делает.

## GuildMemberAddRole

Выдаёт роли при входе пользователя, при условии если конечно настроили командой !config.

## GuildMemberRemove

Делает действие при выходе пользователя.

- Прощается с ним на сервере.

Если бота не настраивали на сервере то ничего не делает.

## Handler

Обрабатывает муты, баны и напоминания. То есть проверяет, не пора ли размутить/разбанить/напомнить пользователя.

## Levels

Здесь находится система уровней за общение.

## Logs

Система логирования сообщений.

- Кто удалил сообщение.
- Кто изменил сообщение.

## Message

Система подсчёта сообщений.

## Reaction

Ставит реакции 👍👎 на сообщения в определённом канале.

## Status

Система статуса сервера и бота в сообщений.

- Обновляется каждые 30 секунд.

Сервер:

- Статус участников. То есть: Ботов, кол-во участников в сети/не активен/не в сети/ не беспокоить и общее количество.
- Количество ролей.
- Количесто эмодзи.
- Защиту сервера.
- Статус каналов. То есть: голосовой онлайн(сколько участников в голосовых каналах), количество сообщений на сервере, количество текстовых и голосовых каналов.

Монитор бота:

- Операционную систему.
- Задержку API.
- Архитектору системы.
- ОЗУ.
- Аптайм системы.

## Voice-Room

Система голосовых комнат.

Когда заходишь в специальный голосовой канал, тебе создаётся голосовой канал со всеми правами и автоматом перенаправляют тебя в него.

При выходе из него он автоматом удаляется.

## afk

Система AFK. Если напишешь сообщение ты автоматически выйдешь из AFK,а если кто-то тебя упомянет бот скажет что вы в AFK.

Чтобы войти в статус AFK нужно написать команду: `!afk <Причина>`

## login

Самый важный модуль. Логинит бота в сеть.