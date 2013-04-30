LessForDle
===================

LessForBitrix - примочка для подключения класса phpless в шаблон bitrix.


### Ссылки
[Автор модуля](http://pafnuty.name/ "ПафНутиЙ")

[Сайт lessphp] (http://leafo.net/lessphp/ "Официальный сайт lessphp")

[Русский сайт LESS] (http://lesscss.ru/ "Официальный сайт LESS")


Для чего это?
-------------------
* Для нормального использования LESS при вёрстке под Bitrix
* И как следствие - для удобной, быстрой и эффективной разработки сайта.

Возможности:
-------------------
* Автоматическая компиляция less при изменении файла, при этом отслеживаются изменения и в импортированных файлах.
* Сжатие выходного css-файла (с возможностью отключать сжатие)
* Вывод ошибок компиляции.

Установка:
-------------------
* Загрузить содержимое папки YOUR_TEMPLATE в папку с шаблоном сайта.
* Где нибудь в начале header.php прописать:
```
<?require_once('less/less.php');?>
```
* По умолчанию подключается файл template_styles.less текущего шаблона сайта.
* При компиляции рядом записывается одноимённый css-файл (который и используется в bitrix по умолчанию).
* При возникновении ошибок - они будут выведены в начале страницы, а компиляция не произойдёт.
* Все настройки (если они нужны) в файле less/less.php