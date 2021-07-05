<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Технические требования 
1. PHP 7.4 
2. Фреймворк:  Symfony 5/Laravel 8. 
3. БД:  MySQL. 
4. Упаковать в docker контейнер. Желательно чтобы после выполнения команд docker-compose build и docker-compose up проект был полностью готов к работе. 
5. Выложить в открытый репозиторий на http://GitHub.com. 
## Общее описание задания 
Необходимо создать RESTfull API для управления лентой новостей. 
При создании формата запросов и ответов используйте все best practices по построению CRUD API на основе RESTfull архитектуры. 
### API должно содержать следующие методы: 
1. Добавление новости. 
2. Редактирование новости. 
3. Удаление новости. 
4. Получение новости по идентификатору. 
5. Поиск новостей. Параметры поиска: <br>
○ Список идентификаторов новостей. <br>
○ Период дат с точностью до дня. <br>
○ Сортировка по полям: заголовок и дата.<br> 
○ Передача параметров пагинации: смещение и лимит.<br> 
6. Получение количества новостей за каждый день в пределах указанного периода. 

#### Внимание! 
Дополнительно нужно реализовать возможность добавления новостей путем передачи их через очередь RabbitMQ. <br> 
Формат сообщения в очереди должен повторять формат сообщения, которое передается через HTTP API. 
### Необходимые поля новости 
1. Уникальный идентификатор. Назначает API. 
2. Заголовок. Длина не больше 255 символов. 
3. Текст. Как-то обрабатывать необязательно. 
4. Автор, в виде текстовой строки. 
5. Дата и время публикации новости. Любой удобный формат.
