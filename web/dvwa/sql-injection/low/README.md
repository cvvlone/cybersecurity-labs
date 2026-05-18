# DVWA SQL Injection - Low

## RU Version

### Цель
Практика эксплуатации SQL-инъекции в DVWA на уровне безопасности LOW с использованием Burp Suite и sqlmap.

### Используемая среда
- Kali Linux
- DVWA (Docker)
- Burp Suite
- sqlmap

### Уязвимость
SQL-инъекция в GET-параметре `id`.

### Используемые инструменты
- Burp Suite
- sqlmap

### Команда sqlmap

```bash
sqlmap -r req.txt -D dvwa -T users --dump --batch
```

### Результат
Успешно обнаружена SQL-инъекция и выполнено извлечение данных из таблицы `dvwa.users`.

### Практикуемые навыки
- Перехват HTTP-запросов
- Тестирование SQL-инъекций
- Работа с sqlmap
- Enumeration базы данных
- Работа с HTTP-запросами

---

## EN Version

### Objective
Practice SQL Injection exploitation on DVWA security level LOW using Burp Suite and sqlmap.

### Environment
- Kali Linux
- DVWA (Docker)
- Burp Suite
- sqlmap

### Vulnerability
SQL Injection in GET parameter `id`.

### Tools Used
- Burp Suite
- sqlmap

### SQLMap Command

```bash
sqlmap -r req.txt -D dvwa -T users --dump --batch
```

### Result
Successfully identified SQL Injection vulnerability and extracted data from `dvwa.users` table.

### Skills Practiced
- HTTP request interception
- SQL Injection testing
- sqlmap usage
- Database enumeration
- Working with HTTP requests
