# Антропов Игорь 588-М1
Предметная область: Интернет-магазин.

## 1 Описание таблиц.

### Описание таблицы "Customers/Клиенты":

![Alt Image 1](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/TableCustomers.png)

* "ID" - уникальный идентификатор заказа;
* "SURNAME" - фамилия;
* "FIRSTNAME" - имя;
* "SECONDNAME" - отчество;
* "EMAIL" - email;
* "NUMBERPHONE" - номер телефона.

### Описание таблицы "Product/Продукт":

![Alt Image 2](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/TableProduct.png)

* "ID" - уникальный идентификатор заказа;
* "NAME" - наименование товара;
* "PRICE" - цена.

### Описание таблицы "StatusOrder/Статус заказа":

![Alt Image 3](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/TableStatusOrder.png)

* "ID" - уникальный идентификатор заказа;
* "NAME" - наименование статуса.

### Описание таблицы "Order/Заказ":

![Alt Image 4](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/TableOrder.png)

* "ID" - уникальный идентификатор заказа;
* "DATE" - наименование товара;
* "ADDRESS" - цена;
* "STATUSORDER_ID" - уникальный идентификатор статуса заказа.

### Описание таблицы "OrderCart/Корзина": 

![Alt Image 5](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/TableOrderCart.png)

* "COUNT" - количество товара;
* "CUSTOMER_ID" - уникальный идентификатор заказчика;
* "PRODUCT_ID" - уникальный идентификатор товара;
* "ORDER_ID" - уникальный идентификатор заказа.

## 2 Генерация данных в таблицы.

Для генерации данных использовался онлайн ресурс: https://www.mockaroo.com.

Пример настроек генератора:

![Alt Image 6](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/ExampleRandom.png)

Пример результата генератора:

![Alt Image 7](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/ExampleRandomResult.png)

[Файл с результатом генерации](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/PRODUCT.xlsx)

## 3 Пример выполнения запросов.

### Пример ROLLUP по 1 атрибуту:

![Alt Image 8](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/RollupProduct.png)

![Alt Image 9](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/RollupProduct1.png)

### Пример ROLLUP по 2 атрибутам:

![Alt Image 10](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/RollupProduct2.png)

![Alt Image 11](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/RollupProduct22.png)

### Пример GROUPING:

![Alt Image 12](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/GroupingProduct.png)

![Alt Image 13](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/GroupingProduct.1.png)

### Пример SUM:

![Alt Image 14](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/SumProduct.png)

![Alt Image 15](https://github.com/IgorAntropov/OnlineStoreDB/raw/dev/media/SumProduct.png1.png.png)

## 4 Заключение.

В результате работы:
* развернута БД Oracle;
* создан ряд таблиц для предметной области "Интернет-магазин";
* создан Docker-контейнер при сборке и запуске которого создается БД. Все используемые запросы находятся в файле [init.sql](https://github.com/IgorAntropov/OnlineStoreDB/blob/master/init.sql);
* для таблицы "Товар" выполнен ряд запросов.

В работе использовались:
* Orcale 11g;
* Docker;
* JetBrains DataGrip.
