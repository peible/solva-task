# Тестовое задание. DevOps
## Linux
Напишите команды для выполнения следующих задач:
- Создание директории devops_test в домашнем каталоге.
- Создание пустого файла readme.txt в созданной директории.
- Показать текущий путь в терминале.
```sh
mkdir devops_test
cd devops_test
touch readme.txt
pwd
```
![linux](/images/linux.png)

## Git
Задание: Выполните следующие действия с использованием Git:
- Создайте новый локальный репозиторий.
- Создайте файл test.txt, добавьте в него текст “Hello DevOps”.
- Закоммитьте изменения с сообщением “Initial commit”.
- Покажите историю коммитов.
```sh
git init
git branch -m main
echo "Hello DevOps" >> test.txt
git add test.txt
git commit -m "Initial commit"
git log
```
![linux](/images/git.png)

## Основы сетевых технологий
Ответьте на вопросы:
- Что такое IP-адрес и для чего он используется?
```
IP-адрес - это уникальный идентификатор устройства. Используется для того, чтобы определять устройства поключенные к сети, и обеспечивать их взаимодействие.
```
- Назовите основные отличия между протоколами TCP и UDP.
```
TCP
Надежный, с установлением соединения, медленнее, сохраняет порядок.
Примеры: HTTP, FTP

UDP
Без установления соединения, быстрее, без гарантий доставки и порядка.
Примеры: DNS, Видео-стримы, Игры
```

## Программирование (Bash или Python)
- Напишите скрипт на Bash или Python, который выводит числа от 1 до 10.
```sh
#!/bin/bash
echo {1..10}
```
```python
print(*range(1, 11))
```
## Логическое мышление
Решите следующую задачу:
- В одном здании находится три лампочки, управляемые тремя выключателями в
другой комнате. Как определить, какой выключатель к какой лампочке относится,
если вы можете зайти в комнату с лампочками только один раз?

```
Если все три лампы — лампы накаливания:
1. Включите первый выключатель и оставьте его включенным на некоторые время. За это время подключенная к этому выключателю лампочка нагреется
2. После выключите первый выключатель и сразу включите второй
3. Теперь зайдите в комнату с лампочками и проверьте
    Та лампа, которая горит, подключена ко второму выключателю
    Та, которая не горит, но теплая, подключена к первому выключателю
    Та, которая не горит и холодная, подключена к третьему выключателю

Если все лампы светодиодные, то скорее всего не почувствуем нагрева
```