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

# Лабораторная работа №2
## Nikita A. Toponen
## RUDN University, 12 September 2022 Moscow, Russia

--- 

# Дискреционное разграничение прав в Linux

---

### Цель выполнения работы

- Получение практических навыков работы в консоли с атрибутами файлов.

- Закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux

---

# Выполнение работы

---

### Выполнение работы

![center](img/1.png)
#### Рис.1 Создание пользователя guest

---

### Выполнение работы

![center](img/2.png)
#### Рис.2 Установка пароля для guest

---

### Выполнение работы

![center](img/3.png)
#### Рис.3 Вход в систему под guest

---

### Выполнение работы

![center](img/4.png)
#### Рис.4 Домашняя директория

---

### Выполнение работы

![center](img/5.png)
#### Рис.5 Определение пользователя

---

### Выполнение работы

![center](img/6.1.png)
#### Рис.6 Имя пользователя, группа, а также группы, куда входит пользователь

---

### Выполнение работы

![center](img/6.2.png)
#### Рис.7 Группы пользователя

---

### Выполнение работы

![center](img/8.png)
#### Рис.8 guest в etc/passwd

---

### Выполнение работы

![center](img/9.png)
#### Рис.9 Существующие в системе директории

---

### Выполнение работы

![center](img/10.png)
#### Рис.10 Расширенные атрибуты

---

### Выполнение работы

![center](img/11.png)
#### Рис.11 Права доступа к новому файлу

---

### Выполнение работы

![center](img/12.png)
#### Рис.12 Изменение аттрибутов

---

### Выполнение работы

![center](img/13.png)
#### Рис.13 Запись в файл без прав

---

### Выполнение работы

![center](img/15.png)
#### Рис.14 Минимально необходимые права для выполнения операций внутри директории dir1

---

### Выводы

В ходе выполнения данной лабораторной работы я:

- Полученил практические навыки работы в консоли с атрибутами файлов.

- На практике закрепил теоретические основы дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux
---

# Спасибо за внимание!