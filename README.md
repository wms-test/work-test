# Задача №1.
Написать класс init, от которого нельзя сделать наследника, состоящий из 3 методов:

- **create()** доступен только для методов класса создает таблицу test, содержащую 5 полей:  

```
- **id** целое, автоинкрементарное  

- **script_name** строковое, длиной 25 символов  

- **start_time** целое  

- **end_time** целое  

- **result** один вариант из 'normal', 'illegal', 'failed', 'success'  
```

- **fill()** доступен только для методов класса заполняет таблицу случайными данными  


- **get()**
доступен извне класса
выбирает из таблицы test, данные по критерию: result среди значений 'normal' и 'success'
В конструкторе выполняются методы create и fill


Задание должно быть выполнено с использованием классов ZendFramework с поддержкой исключений.
Весь код должен быть прокомментирован в стиле **PHPDocumentor'а**.

# Задача №2.

Знания MySQL + оптимизировать запросы
Имеется 3 таблицы: info, data, link, есть запрос для получения данных:
select * from data,link,info where link.info_id = info.id and link.data_id = data.id
предложить варианты оптимизации:
таблиц
запроса.
Запросы для создания таблиц:
```
CREATE TABLE `info` (
        `id` int(11) NOT NULL auto_increment,
       `name` varchar(255) default NULL,
        `desc` text default NULL,
        PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=cp1251;

CREATE TABLE `data` (
        `id` int(11) NOT NULL auto_increment,
        `date` date default NULL,
        `value` INT(11) default NULL,
        PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=cp1251;

CREATE TABLE `link` (
        `data_id` int(11) NOT NULL,
        `info_id` int(11) NOT NULL
) ENGINE=MyISAM DEFAULT CHARSET=cp1251;
```

# Задача №3.
Создать скрипт, который в папке /datafiles найдет все файлы, имена которых состоят из цифр и букв латинского алфавита, имеют расширение ixt и выведет на экран имена этих файлов, упорядоченных по имени.
Задание должно быть выполнено с использованием регулярных выражений.
Весь код должен быть прокомментирован в стиле PHPDocumentor'а.

# Задача №4.
Написать скрипт закачивания страницы www.bills.ru, из страницы извлечь даты, заголовки, ссылки в блоке "события на долговом рынке", сохранить в таблицу bills_ru_events, имеющей такую структуру:

id
целое, автоинкрементарное
date
в формате год-месяц-день часы:минуты:секунды
title
строковое не более 230 символов
url
строковое не более 240 символов, уникальное
Весь код должен быть прокомментирован в стиле PHPDocumentor'а.

# Задача №5.
Cоздать 3 кнопки с названиями 1, 2, 3, расположенные друг над другом.

Начальный вид: 


Нажали на любую кнопку, меняется порядок на:


Нажали на любую кнопку, меняется порядок на: 


Нажали на любую кнопку, меняется порядок на: 


Код должен быть написан с ипользованием библиотеки jQuery.
______________________________________________________________
```
Для выполнения тестовых задач вам обязательно понадобится: 
- Zend Framework, Zend Studio (http://www.zend.com/en/downloads/)
- jQuery (http://docs.jquery.com/Downloading_jQuery)
- MySQL Server 5.x (http://www.mysql.com/downloads/mysql/) 
- PHP 5.x (http://www.php.net/downloads.php)
- Apache 2.x (http://httpd.apache.org/)
```