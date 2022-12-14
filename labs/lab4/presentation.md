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

# Лабораторная работа №4
## Nikita A. Toponen
## RUDN University, 25 September 2022 Moscow, Russia

--- 

# Дискреционное разграничение прав в Linux. Расширенные атрибуты

---

### Цель выполнения работы

- Получение практических навыков работы в консоли с расширенными атрибутами файлов.

- Закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux.

---

# Выполнение работы

---

### Выполнение работы

![w:900 h:200 center](img/1.png)
#### Рис.1 Определение расширенных атрибутов файла file1

---

### Выполнение работы

![w:1000 h:200 center](img/2.png)
#### Рис.2 Установление прав на файл file1

---

### Выполнение работы

![w:1000 h:200 center](img/3.png)
#### Рис.3 Установление расширенных прав на файл file1 пользователем guest

---

### Выполнение работы

![w:1000 h:200 center](img/4.png)
#### Рис.4 Установление расширенных прав на файл file1 суперпользователем

---

### Выполнение работы

![w:1000 h:200 center](img/5.png)
#### Рис.5 Проверка расширенных прав на файл file1

---

### Выполнение работы

![w:1000 h:200 center](img/6.png)
#### Рис.6 Выполнение дозаписи в файл с атрибутом a

---

### Выполнение работы

![w:1000 h:300 center](img/7.png)
#### Рис.7 Удаление и перезапись файла с атрибутом a

---

### Выполнение работы

![w:1000 h:200 center](img/8.png)
#### Рис.8 Изменения прав на файл с атрибутом a

---

### Выполнение работы

![w:1000 h:450 center](img/9.png)
#### Рис.9 Повторение операций без атрибута a

---

### Выполнение работы

![w:1000 h:450 center](img/10.png)
#### Рис.10 Повторение операций с атрибутом i

---

### Выводы

В ходе выполнения данной лабораторной работы я:

- Повысил свои навыки использования интерфейса командой строки (CLI)

- Познакомился на примерах с тем, как используются основные и расширенные атрибуты при разграничении доступа

- На практике закрепил теоретические основы дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux

---

# Спасибо за внимание!
