# Асинхронный парсер Циан

- AsyncIO
- SQLAlchemy
- PostgreSQL
- AIOHTTP

## Структура запроса xlsx с доступными предложениями
```
https://spb.cian.ru/export/xls/offers/
    ?bbox=59.8036975013%2C29.9261539416%2C60.0717561528%2C30.6629245715&
    currency=2&
    deal_type=rent&
    engine_version=2&
    maxprice=35000&
    offer_type=flat&
    p=18&
    region=2&
    room1=1&
    room2=1&
    room3=1&
    room4=1&
    room5=1&
    room6=1&
    type=4
```
### Параметры
```bbox``` - Координаты квадрата для поиска \
```currency``` - Валюта (2 - RUB) \
```deal_type``` - Тип предложения (rent - длительная аренда) \
```engine_version``` - Версия движка (по умолчанию - 2) \
```maxprice``` - Максимальная цена в выбранной валюте \
```offer_type``` - Тип недвижимости (flat - квартира) \
```p``` - Номер страницы \
```region``` - ? (по умолчанию - 2) \
```room1``` - Включать в поиск однокомнатные квартиры \
```room2``` - Включать в поиск двухкомнатные квартиры \
```room3``` - Включать в поиск трёхкомнатные квартиры \
```room4``` - Включать в поиск четырёхкомнатные квартиры \
```room5``` - Включать в поиск пятикомнатные квартиры \
```room6``` - Включать в поиск шестикомнатные квартиры \
```type``` - ? (по умолчанию - 4) 

## TODO:

- [ ] Определить все параметры и значения, которые могут подаваться в запрос \
- [ ] Понять назначение type в запросе