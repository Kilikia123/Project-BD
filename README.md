# Проект по БД

## Концептуальная модель
![conceptual_model drawio (1)](https://user-images.githubusercontent.com/65976385/161466593-456fee18-08a9-48bb-8e51-66d5382adba6.svg)


## Логическая модель
![logic_model drawio](https://user-images.githubusercontent.com/65976385/161466611-3b0fc902-7189-4a45-90db-4c6b7c92246b.svg)

## Физическая модель

**Заказ**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_order   |  INT | 4|
ID_employee   | INT | 4| 
ID_client   | INT | 4|

**Описание заказов**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_order   |  INT | 4|
ID_product   | INT | 4| 
amount_product   | INT | 4|

**Ассортимент товаров**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_product   |  INT | 4|
description   | VARCHAR(700) | 701| 
price_pr   | INT | 4|

**Клиент**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_client   |  INT | 4|
email   | VARCHAR(40) | 41| 
phone_number   | INT | 4|
user_name   | VARCHAR(20) | 21|
user_last_name   | VARCHAR(20) | 21|
user_birth   | DATE | 3|
card_number   | VARCHAR(40) | 41|

**Оплата заказа**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_order   |  INT | 4|
total_amount   | INT | 4| 
is_paid   | BIT | |
delivery_method   |  VARCHAR(20) | 21|
payment_method   | VARCHAR(20) | 21| 

**Сотрудники**
Field name | Data type | Size (bytes)|
------ | ------|------|
ID_employee   |  INT | 4|
salary   | INT | 4| 
employee_name   | VARCHAR(20) | 21|
employee_last_name   | VARCHAR(20) | 21|
employee_birth   | DATE | 3| 
phone_number  | INT | 4|
card_number   |  VARCHAR(40) | 41|
