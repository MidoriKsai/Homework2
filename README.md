# АНАЛИЗ ДАННЫХ В РАЗРАБОТКЕ ИГР
Отчет по лабораторной работе #2 выполнила:
- Миногина Дарья Алексеевна
- РИ-230932
  
Отметка о выполнении заданий:

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |
| Задание 4 | * |(дополнительно) |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Выбрать одну из игровых переменных в игре СПАСТИ РТФ: Выживание (HP, SP, игровая валюта, здоровье и т.д.), описать её роль в игре, условия изменения / появления и диапазон допустимых значений. Построить схему экономической модели в игре и указать место выбранного ресурса в ней.
- Задание 2.
- С помощью скрипта на языке Python заполнить google-таблицу данными, описывающими выбранную игровую переменную в игре “СПАСТИ РТФ:Выживание”. Средствами google-sheets визуализировать данные в google-таблице для наглядного представления выбранной игровой величины. Описать характер изменения этой величины недостатки в реализации этой величины и предложить до 3-х вариантов модификации условий работы с переменной, чтобы сделать игровой опыт лучше.
- Задание 3.
- Настроить на сцене Unity воспроизведение звуковых файлов, описывающих динамику изменения выбранной переменной.
- Задание 4.
- Придумать как использовать к игре указанной выше этот способ.
- Выводы.
- ✨Magic✨

## Цель работы
Научиться передавать в Unity данные из Google Sheets с помощью Python.

## Задание 1
### Выбрать одну из игровых переменных в игре СПАСТИ РТФ: Выживание (HP, SP, игровая валюта, здоровье и т.д.), описать её роль в игре, условия изменения / появления и диапазон допустимых значений. Построить схему экономической модели в игре и указать место выбранного ресурса в ней.

#### Для начала нужно настроить всё, что пригодится для работы с google-таблицами

- Настроить доступ к google-таблице по api

![API](https://github.com/MidoriKsai/Homework2/blob/main/API.png)

- Сгенерировать данные с помощью Python и передать их в google-таблицу
- Создать ключ API для передачи данных из google-таблицы в Unity

### Анализ переменной "игровая валюта" в игре "СПАСТИ РТФ: Выживание"

#### **Роль в игре:**

Игровая валюта играет ключевую роль, как основное средство стимулирования игрока, связанное с прогрессом и поддержанием боеспособности персонажа.

#### **Условия появления и диапазон допустимых значений:**
  
- **Убийство зомби**: За каждого убитого зомби игрок получает определенное количество денег. С увеличением уровня волны может увеличиваться награда за более сильных зомби, так например: за убийство зомби первой волны игрок получает 1 монету, за убийство зомби 4 волны, 4 монеты и так далее

- **Сундуки с золотом**: На карте игрок может найти сундуки, содержащие золото, которое может быть переведено в монеты, после сбора

- **Улучшение "Коллектор"**: С помощью данного усиления, за каждое попадание игрок может получить небольшой доход

- **Просмотр рекламы**: Можно получить как монеты напрямую, так и сундуки с монетами

Больше всего монет за раз можно получить за просмотр рекламы (от 50 до 100). За каждого зомби можно получить от 1 монеты и более (цена зависит от волны, цена = волна). Именно в игре самым щедрым на монеты является сундук. Самый минимальный доход идет от усиления "Коллектор"

#### **Схема экономической модели**

## Задание 2
###  С помощью скрипта на языке Python заполнить google-таблицу данными, описывающими игровую валюту в игре “СПАСТИ РТФ:Выживание”. Средствами google-sheets визуализировать данные в google-таблице (построить график / диаграмму и пр.) для наглядного представления выбранной игровой величины. Описать характер изменения этой величины, описать недостатки в реализации этой величины (например, в игре может произойти условие наступления эксплойта) и предложить до 3-х вариантов модификации условий работы с переменной, чтобы сделать игровой опыт лучше..

- Запустить Unity и с помощью VSC вывести "Hello World" на экран
![Hello World Unity](https://github.com/MidoriKsai/Homework/blob/main/HelloWorld_unity.png)

## Задание 3
### Оформить отчет в виде документации на github (markdown-разметка).

  ![Github](https://github.com/MidoriKsai/Homework/blob/main/Github_hw.png)

## Задание 4
###  Какую сущность(и) мы бы могли "обучить" ML-Agent-ом для того, чтобы создать более качественный игровой опыт?

- К сожалению, не часто играю в шутеры, поэтому дальше 3 волны пройти не получилось, могу предложить зомби-водителей, которых можно остановить только взрывом(бомбой), но, опять же, не уверена, может уже такие есть, просто я до них не дошла.



## Выводы

Мы скачали нужное ПО и научились запускать код, через разные инструменты.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
