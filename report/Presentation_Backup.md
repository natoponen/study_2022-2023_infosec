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

# Системы резервного копирования
## Nikita A. Toponen
## RUDN University, 27 September 2022 Moscow, Russia

--- 


### Определение

Система резервного копирования (СРК) определяется:
- Политикой резервного копирования.
- Регламентом резервного копирования, определяемого политикой.
- Инструментальной реализацией.

---

### Процесс резервного копирования
  
- Периодический запуск копирования.
- Запуск восстановления по требованию.
- Тестирование процесса копирования

---

### Архитектура и работа системы резервного копирования

![w:700 h:475 center](img/1.png)
#### Рис.1 Архитектура системы резервного копирования

---

### Классификация резервного копирования

По полноте сохраняемой информации
- Полное резервирование (Full backup)
- Добавочное резервирование (Incremental backup) 
- Разностное резервирование (Differential backup)
- Выборочное резервирование (Selective backup) 

По способу доступа к носителю
- Оперативное резервирование (Online backup)
- Автономное резервирование (Offline backup)


---

# Технологии резервного копирования

---

### Внесетевое копирование

![w:700 h:475 center](img/2.png)
#### Рис.2 Организация внесетевого копирования

---

### Внесерверное копирование

![w:700 h:475 center](img/3.png)
#### Рис.3 Организация внесерверного копирования

---

### Репликация

![w:700 h:225 center](img/4.png)
#### Рис.4 Организация внесерверного копирования

![w:700 h:225 center](img/5.png)
#### Рис.5 Организация внесерверного копирования

---

# Выводы

---

### Библиография

1. Медведовский И.Д., Семьянов П.В., Платонов В.В. Атака через Internet. — НПО "Мир и семья-95",  1997. — URL: http://bugtraq.ru/library/books/attack1/index.html
2. Медведовский И.Д., Семьянов П.В., Леонов Д.Г.  Атака на Internet. — Издательство ДМК, 1999. — URL: http://bugtraq.ru/library/books/attack/index.html
3. Запечников С. В. и др. Информационн~пасность открытых систем. Том 1. — М.: Горячаая линия -Телеком, 2006.
4. Статья в электронном журнале «Хабр»: «Система резервного копирования» https://habr.com/ru/post/421251/
5. Статья в электронном журнале TADVISER: «Система резервного копирования» https://www.tadviser.ru/index.php/Статья:Система_резервного_копирования

---

# Спасибо за внимание!