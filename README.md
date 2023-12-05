# Проект парсинга pep

## Описание
Парсер собирает данные обо всех PEP документах, сравнивает статусы и записывает их в файл, также реализованы сбор информации о статусе версий, скачивание архива с документацией и сбор ссылок о новостях в Python.

## Технолгии
- Python 3.9
- BeautifulSoup 4.9
- Prettytable 2.1

## Запуск проекта
Клонировать репозиторий и перейти в директорию проекта:
```
git clone https://github.com/KonstantinSKS/bs4_parser_pep.git
```
```
cd bs4_parser_pep
```
Cоздать и активировать виртуальное окружение:
```
python -m venv venv
```
### Команда для Windows:
```
source venv/Scripts/activate
```
### Для Linux и macOS:
```
source venv/bin/activate
```
Установить зависимости из файла requirements.txt:
```
python3 -m pip install --upgrade pip
```
```
pip install -r requirements.txt
```
Ознакомиться со справкой или запустить проект в нужном режиме:
```
python main.py --help
```
или
```
python main.py [-h] [-c] [-o {pretty,file}] {whats-new, latest-versions, download, pep}
```
Полный список аргументов:
```
usage: main.py [-h] [-c] [-o {pretty,file}] {whats-new,latest-versions,download,pep}

Парсер документации Python

positional arguments:
  {whats-new,latest-versions,download,pep}
                        Режимы работы парсера

optional arguments:
  -h, --help            show this help message and exit
  -c, --clear-cache     Очистка кеша
  -o {pretty,file}, --output {pretty,file}
                        Дополнительные способы вывода данных
```
