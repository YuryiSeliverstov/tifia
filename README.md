# Tifia

По базе данных:
Во многих таблицах нет индексов по искомым полям
например в "accounts" нет индекса по client_uid, если по login тоже идёт поиск тоже
соотв. также нужно проставить (у меня не получилось, написало нет прав)

Далее таблица "trades", нужен индекс по login, open_time, close_time, в идеале вообще хранить дату не в datetime 
а в integer'е банально быстрее в разы и более универсален.

Прикрепил два архива (7-zip, zip) с локальной копии, так как почему то на GitHub, 
проект полностью заливаться не хочет....

Вызов из консоли (проверял на винде, wamp64 PHP 7.3):

php yii site/tree

php yii site/partner 82824897 "2019-01-10 00:00:00" "2019-01-20 00:00:00"
