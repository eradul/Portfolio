Краткое ТЗ:
Бизнес-задача: анализ взаимодействия пользователей с карточками Яндекс.Дзен;

Частота использования дашборд: не реже, чем раз в неделю;

Основной пользователь дашборда: менеджеры по анализу контента;

Состав данных для дашборда:

история событий по темам карточек (два графика - абсолютные числа и процентное соотношение);
разбивка событий по темам источников;
таблица соответствия тем источников темам карточек;
Параметры данных для группировки:

Дата и время;
Тема карточки;
Тема источника;
Возрастная группа;
Характер данных:

История событий по темам карточек — абсолютные величины с разбивкой по минутам;
Разбивка событий по темам источников — относительные величины (% событий);
Соответствия тем источников темам карточек - абсолютные величины;
Важность: все графики имеют равную важность;

Источники данных для дашборда: агрегирующая таблица dash_visits со структурой:

record_id — первичный ключ,
item_topic — тема карточки,
source_topic — тема источника,
age_segment — возрастной сегмент,
dt — дата и время,
visits — количество событий.
Таблица хранится в специально подготовленной для вас базе данных zen;

Частота обновления данных: один раз в сутки, в полночь по UTC;

Макет дашборда
![Макет дашборда]()
