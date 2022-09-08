---
# Front matter
lang: ru-Ru
title: "Лабораторная работа №1"
subtitle: "Установка дистрибутива CentOS"
author: "Топонен Никита Андреевич"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: xelatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков установки операционной системы CentOS на виртуальную машину, а также настройка минимально необходимого окружения для дальнейшей работы.

# Задание

Установить и настроить дистрибутив CentOS на виртуальную машину, а также установить дополнения необходимые для дальнейшей работы.

# Теоретическое введение

Для выполнения данной лабораторной нет специальной теории. Необходимы общие знания в области компьютерных наук.

# Выполнение лабораторной работы

Первым шагом необходимо создать виртуальную машины в VirtualBox. Для этого выбираем ***Машина -> Создать***.

![Создание виртуальной машины](img/scr1.png){#fig:001}

Затем указываем объем оперативной памяти, выделенный виртуальной машине. В моём случае он равен 2048МБ.

![Объем оперативной памяти](img/scr2.png){#fig:002}

Далее создаем новый динамический виртуальный жесткий диск типа VDI и задаем его размер.

![Создание виртуального жесткого диска](img/scr3.png){#fig:003}

![Тип виртуального жесткого диска](img/scr4.png){#fig:004}

![Формат хранения](img/scr5.png){#fig:005}

В VirtualBox заходим в ***Настройки -> Носители*** и добавляем новый привод оптических дисков, где выбираем заранее скачанный образ выбранной операционной системы.

![Выбор образа операционной системы](img/scr6.png){#fig:006}

После этого запускаем виртуальную машину и начинаем установку ОС.

![Старт установки ОС](img/scr7.png){#fig:007}

По ходу начальной настройки ОС перед ее установкой нужно выполнить несколько шагов.

- Выбрать язык

![Выбор языка](img/scr9.png){#fig:008}

- Настроить часовой пояс.

![Выбор часового пояса](img/scr10.png){#fig:009}

- Выбрать пакет предустановленных программ.

![Выбор пакета программ](img/scr11.png){#fig:010}

- Отключить KDUMP.

![Отключение KDUMP](img/scr12.png){#fig:011}

- Включить сетевое соединение, с именем узла natoponen.localadmin.

![Включение сетевого соединения](img/scr13.png){#fig:012}

- Установить пароль для root.

![Задание пароля для root](img/scr14.png){#fig:013}

- Создать пользователя с правами администратора.

![Создание пользователя](img/scr15.png){#fig:014}

- Правильно перезагрузить систему.

![Перезагрузка системы](img/scr16.png){#fig:015}

- Принять лицензионное соглашение.

![Принятие лицензии](img/scr17.png){#fig:016}

После выполнения данных шагов мы попадаем на рабочий стол нашей виртуальной машины. Для более удобной работы с машиной нужно подключить образ диска дополнительной гостевой ОС. Чтобы сделать это, необходимо в меню ***Устройства*** окна VirtualBox выбрать опцию подключения диска дополнительной гостевой ОС. Появится всплывающее окно, в котором можно запустить данный процесс.

![Запуск подключения диска дополнительной гостевой ОС](img/scr19.png){#fig:019}

На этом установка CentOS на виртуальную машину завершается.

## Домашнее задание

С помощью утилит *dmesg* и *grep* найдем некоторую информацию о системе.

1. Версия ядра Linux: 3.10.0-1160
2. Частота процессора: 2095.990 MHz
3. Модель процессора: AMD Ryzen 5 5500U with Radeon Graphics
4. Объем доступной памяти: 2013292k
5. Тип обнаруженного гипервизора: KVM
6. Тип файловой системы корневого раздела: XFS

![Информация о системе](img/scr22.png){#fig:020}

![Информация о системе](img/scr23.png){#fig:021}

# Выводы

В ходе выполнения данной лабораторной работы я приобрел практические навыки установки операционной системы CentOS на виртуальную машину, а также знания по настройке минимально необходимого окружения для дальнейшей работы.


# Список литературы

- <code>[Кулябов Д. С., Королькова А. В., Геворкян М. Н Лабораторная работа №1](https://esystem.rudn.ru/mod/folder/view.php?id=892013)</code>