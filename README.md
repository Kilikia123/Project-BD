# Проект по БД "Розничный магазин строительных материалов"

## Концептуальная модель
![conceptual_model drawio (1)](https://user-images.githubusercontent.com/65976385/167299086-89599ea3-c212-4c85-9149-03676d0fc308.svg)


## Логическая модель
![logic_model drawio (1)](https://user-images.githubusercontent.com/65976385/167299095-90a7bab0-08ad-45a3-b15b-6425adc899f2.svg)

## Физическая модель

**Описание заказ**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_order |Индентификатор заказа  |  INT | NOT NULL|
ID_client  | Индентификатор клиента | INT | NOT NULL|
amount_product  | Кол-во этого товара | INT | NOT NULL|

**Ассортимент товаров**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_product |Индентификатор товара  |  INT | NOT NULL|
description |Описание товара   | VARCHAR(700) | | 
price_pr  |Цена товара | INT | |

**Клиент**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_client| Индентификатор клиента   |  INT | NOT NULL|
email  | Почта клиента| VARCHAR(40) | | 
phone_number | Номер телефона клиента  | INT ||
user_name  | Имя клиента | VARCHAR(20) | |
user_last_name | Фамилие клиента | VARCHAR(20) | |
user_birth | Дата рождения клиента | DATE | |
card_number | Банковская карта клиента | VARCHAR(40) | |

**Заказ**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_order |Индентификатор заказа |  INT | NOT NULL|
ID_client |Индентификатор клиента |  INT | NOT NULL|
total_amount | Общая сумма заказа | INT | NOT NULL| 
is_paid | Оплачен ли заказ | BIT | NOT NULL|
delivery_method |  Способ доставки |  VARCHAR(20) | NOT NULL|
payment_method | Способ оплаты | VARCHAR(20) | NOT NULL| 
