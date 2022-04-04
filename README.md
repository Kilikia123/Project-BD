# Проект по БД "Розничный магазин строительных материалов"

## Концептуальная модель
![conceptual_model drawio (1)](https://user-images.githubusercontent.com/65976385/161466593-456fee18-08a9-48bb-8e51-66d5382adba6.svg)


## Логическая модель
![logic_model drawio (1)](https://user-images.githubusercontent.com/65976385/161645735-630178c4-9f3c-4abb-a9d3-9ccb91c9699e.svg)

## Физическая модель

**Заказ**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_order |Индентификатор заказа  |  INT | NOT NULL|
ID_employee |Индентификатор сотрудника  | INT | NOT NULL| 
ID_client  | Индентификатор клиента | INT | NOT NULL|

**Описание заказов**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_order |  Индентификатор заказа |  INT | NOT NULL|
ID_product | Индентификатор товара  | INT | NOT NULL| 
amount_product | Кол-во товара   | INT | NOT NULL|

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

**Оплата заказа**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_order |Индентификатор заказа |  INT | NOT NULL|
total_amount | Общая сумма заказа | INT | NOT NULL| 
is_paid | Оплачен ли заказ | BIT | NOT NULL|
delivery_method |  Способ доставки |  VARCHAR(20) | NOT NULL|
payment_method | Способ оплаты | VARCHAR(20) | NOT NULL| 

**Сотрудники**
Field name |Description | Data type | Restrictions|
------ | ------|------|------|
ID_employee | Индентификатор сотрудника  |  INT | NOT NULL|
salary  | Зарплата сотрудника | INT | | 
employee_name | Имя сотрудника | VARCHAR(20) | |
employee_last_name |Фамилие сотрудника  | VARCHAR(20) | |
employee_birth |Дата рождения сотрудника  | DATE | | 
phone_number | Номер телефона  | INT | |
card_number  | Банковская карта |  VARCHAR(40) | |
