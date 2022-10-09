---
marp: true
paginate: true
author: Nikita A. Toponen
theme: default
math: mathjax
---
<style>
section::after {
  content: attr(data-marpit-pagination) ' / ' attr(data-marpit-pagination-total);
}
img[alt="center"] {
     display: block;
     margin: 0 auto;
}
h1 {
    font-size: 60px;
    text-align: center;
}
h2 {
    font-size: 30px;
    text-align: left;
    position: relative;
    left: -2em;
    line-height: 0px;
    top: 8em;
}
h3 {
    font-size: 40px;
    text-align: left;
    position: relative;
    left: -0.5em;
    bottom: 0.2em;
}
h4 {
    font-size: 25px;
    text-align: center;
    position: relative;
    left: -0.5em;
    bottom: 0.2em;
}
</style>

# Лабораторная работа №6
## Nikita A. Toponen
## RUDN University, 9 October 2022 Moscow, Russia

--- 

# Мандатное разграничение прав в Linux

---

### Цель выполнения работы

- Развить навыки администрирования ОС Linux

- Получить первое практическое знакомство с технологией SELinux

- Проверить работу SELinx на практике совместно с веб-сервером Apache

---

# Выполнение работы

---

### Выполнение работы

![w:900 h:400 center](img/3.png)
#### Рис.1 Режим и политика SELinux

---

### Выполнение работы

![w:1000 h:500 center](img/4.png)
#### Рис.2 Запуск Apache web server

---

### Выполнение работы

![w:1000 h:400 center](img/5.png)
#### Рис.3 Контекст безопасности Apache web server

---

### Выполнение работы

![w:1000 h:500 center](img/6.png)
#### Рис.4 Текущее состояние переключателей SELinux для Apache

---

### Выполнение работы

![w:1000 h:200 center](img/8.png)
#### Рис.5 Тип файлов и поддиректорий

---

### Выполнение работы

![w:1000 h:300 center](img/9.png)
#### Рис.6 Создание файла test.html

---

### Выполнение работы

``` html
<html>
<body>test</body>
</html>
```
#### Текст файла test.html

---

### Выполнение работы

![w:1000 h:200 center](img/10.png)
#### Рис.7 Контекст файла test.html

---

### Выполнение работы

![w:1000 h:400 center](img/11.png)
#### Рис.8 Веб страница

---

### Выполнение работы

![w:1000 h:200 center](img/12.png)
#### Рис.9 Контекст файла test.html

---

### Выполнение работы

![w:1000 h:250 center](img/13.png)
#### Рис.10 Изменения контекста файла test.html

---

### Выполнение работы

![w:1000 h:350 center](img/14.png)
#### Рис.11 Доступ к странице запрещен

---

### Выполнение работы

![w:1000 h:350 center](img/15.png)
#### Рис.12 Логи веб сервера

---

### Выполнение работы

![w:1000 h:350 center](img/16.png)
#### Рис.13 Audit логи

---

### Выполнение работы

![w:1000 h:450 center](img/17.png)
#### Рис.14 Смена порта

---

### Выполнение работы

![w:1000 h:450 center](img/18.png)
#### Рис.15 Запуск на 81 порту

---

### Выполнение работы

![w:1000 h:350 center](img/19.png)
#### Рис.16 Установление порта

---

### Выполнение работы

![w:1000 h:500 center](img/20.png)
#### Рис.17 Работа веб сервера на 81 порту

---

### Выполнение работы

![w:1000 h:350 center](img/21.png)
#### Рис.18 Возвращение к 80 порту

---

### Выполнение работы

![w:1000 h:350 center](img/22.png)
#### Рис.19 Удаление файла страницы

---

### Выполнение работы

![w:1000 h:350 center](img/23.png)
#### Рис.20 Результат работы сервера после удаления

---

### Выводы

В ходе выполнения данной лабораторной работы я:

- Развил навыки администрирования ОС Linux

- Получил первое практическое знакомство с технологией SELinux

- Проверил работу SELinx на практике совместно с веб-сервером Apache

---

# Спасибо за внимание!
