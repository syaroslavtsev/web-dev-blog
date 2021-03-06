<p align="center">
  <a href="http://nginx.org/ru/" target="_blank">
    <img  style="max-width:100%;"
          alt="alt Nginx"
          src="https://raw.github.com/uran1980/web-dev-blog/master/Nginx/images/nginx-logo.png" />
  </a>
</p>

**[Nginx (engine x)](http://nginx.org/ru/)** — свободный Веб-сервер и почтовый прокси-сервер, работающий на Unix-подобных операционных системах (тестировалась сборка и работа на FreeBSD, GNU/Linux, Solaris, Mac OS X). С версии 0.7.52 появилась бинарная сборка под Microsoft Windows.

Разрабатывается **[Игорем Сысоевым](http://ru.wikipedia.org/wiki/%D0%A1%D1%8B%D1%81%D0%BE%D0%B5%D0%B2,_%D0%98%D0%B3%D0%BE%D1%80%D1%8C_%D0%92%D0%BB%D0%B0%D0%B4%D0%B8%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B8%D1%87)** с 2002-го года для компании Rambler и постоянно модернизируется. Осенью 2004 года вышел первый публично доступный релиз.

***
**ЗАМЕЧАНИЕ:**
Nginx это не замена web-серверу **[Apache](http://ru.wikipedia.org/wiki/Apache)** (у которого огромное количество модулей позволяющих использовать его практически с любым окружением), а специализированный веб-сервер которого в некоторых случаях вполне достаточно. Также при необходимости его можно настроить для работы в связке с апачем.
***

### Nginx позволяет:
* снизить потребление системных ресурсов на сервере (меньше памяти, меньше нагрузки на процессор),
* осуществлять проксирование и балансировку трафика между несколькими бэкэнд серверами с приоритетами и кэшированием ответов,
* ограничивать полосы пропускания для пользователей,
* напрямую забирать данные из **[memcached](http://www.uran1980.com/myfolio/2009/05/19/memcached/)** ,
* осуществлять быструю раздачу статики. Возможность раздачи через X-Accel-Redirect, то есть когда контроль доступа к файлу работает на стороне приложения,
* по сравнению с **[lighttpd](http://ru.wikipedia.org/wiki/Lighttpd)** — вменяемый конфиг.


### Основные недостатки:
не работают апачевский .htaccess (это решается или использованием в качестве бэкэнда apache или описыванием rewrite правил в конфиге nginx)


## Ссылки
* **[http://nginx.org](http://nginx.org/ru/)** - официальный сайт
* **[http://nginx.org/ru/docs/](http://nginx.org/ru/docs/)** - официальная документация по nginx на русском
* **[http://ru.wikipedia.org/wiki/Nginx](http://ru.wikipedia.org/wiki/Nginx)** - описание на Википедии
* **[http://wiki.nginx.org/Main](http://wiki.nginx.org/Main)** - англоязычная wiki по nginx
* **[htaccess-конвертер для nginx](http://winginx.ru/htaccess)** - (русс.)
* **[Еще один htaccess-конвертер для nginx](http://www.anilcetin.com/convert-apache-htaccess-to-nginx/)** - (англ.)


## См. также
* **[Конфигурация Nginx и подводные камни](https://github.com/uran1980/web-dev-blog/blob/master/Nginx/nginx-pitfalls.md)**
* **[Nginx+php-fpm+perl под Debian Squeeze](http://habrahabr.ru/post/164401/)** - очень хорошая статья на хабре по правильной настройке nginx
* **[Memcached](https://github.com/uran1980/web-dev-blog/blob/master/Memcached/memcached.md)**
