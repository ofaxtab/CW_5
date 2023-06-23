# Сборщик вакансий с hh.ru

Проект предназначен для получения вакансий с сайта hh.ru по конкретным работадателям.

---
### Requirements 
certifi==2023.5.7  
charset-normalizer==3.1.0  
idna==3.4  
psycopg2==2.9.6  
requests==2.31.0  
urllib3==2.0.3

### Перед запуском

Необходимо установить postgres на компьютер и создать дефолтную базу данных с названием "postgres".  
Пароль от базы данных необходимо записать в файл database.ini в ключ "password".

### Методы
- `get_companies_and_vacancies_count()`: получает список всех компаний и количество вакансий у каждой компании.
- `get_all_vacancies()`: получает список всех вакансий с указанием названия компании, названия вакансии и зарплаты и ссылки на вакансию.
- `get_avg_salary()`: получает среднюю зарплату по вакансиям.
- `get_vacancies_with_higher_salary()`: получает список всех вакансий, у которых зарплата выше средней по всем вакансиям.
- `get_vacancies_with_keyword()`: получает список всех вакансий, в названии которых содержатся переданные в метод слова, например “python”.