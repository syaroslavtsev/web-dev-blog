<p align="center">
  <img  style="max-width:100%;"
        alt="alt Memcached"
        src="https://raw.github.com/uran1980/web-dev-blog/master/Memcached/images/memcached_banner75.jpg">
</p>

Memcached
=========
**[Memcached](http://memcached.org/)** — это высоко-производительная распределенная система кеширования данных в оперативной памяти, предназначенная для повышения производительности динамических web-приложений и снижения нагрузки на базу данных.

С помощью клиентской библиотеки (для Perl, PHP, Python, Java и др.) memcached позволяет кэшировать данные в оперативной памяти одного или нескольких из множества доступных серверов. Распределение реализуется путем сегментирования данных по значению хэша ключа по аналогии с гнездами хэш-таблицы. Клиентская библиотека используя ключ данных вычисляет хэш и использует его для выбора соответствующего сервера. Ситуация сбоя сервера трактуется как промах кэша, что позволяет повышать отказоустойчивость комплекса за счет наращивания количества memcached серверов и возможности производить их горячую замену.

В **[API memcached](http://code.google.com/p/memcached/wiki/NewCommands)** есть только базовые функции: выбор сервера, установка и разрыв соединения, добавление, удаление, обновление и получение объекта. Для каждого объекта устанавливается время жизни, от 1 секунды до бесконечности. При переполнении памяти более старые объекты автоматически удаляются. Для PHP также есть уже готовые библиотеки PECL для работы с memcached, которые дают дополнительную функциональность.

Сервер memcached был разработан для сайта **LiveJournal** с целью снижения нагрузки на сервера баз данных.

## Ссылки
* **[memcached.org/](http://memcached.org/)** - официальный сайт проекта
* **[https://github.com/memcached](https://github.com/memcached)** - страничка на **GitHub**
* **[http://ru.wikipedia.org/wiki/Memcached](http://ru.wikipedia.org/wiki/Memcached)** - описание на Википедии

## См. также
* **[Обзор Memcached](https://github.com/uran1980/web-dev-blog/blob/master/Memcached/memcached-overview.md)**
* **[Nginx](https://github.com/uran1980/web-dev-blog/blob/master/Nginx/nginx.md)**
