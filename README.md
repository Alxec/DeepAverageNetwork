# Deep Average Network

The task is to build an MLP model that would categorize sentiments of tweets (negative, positive, or neutral). All comments are in English.

## Как сделать домашку
- Склонируйте этот репозиторий
- Установите зависимости
- Сделайте задание
- Заполните [форму](https://form.asana.com/?k=eVYSc3YoLX_Wrr9lAGCkTA&d=1200876361410536)

## Описание задания
В этой домашке мы будет классифицировать твиты на 3 тональности.  
Вы будете использовать предобученные эмбеддинги слов, так что для начала обязательно нужно посмотреть [туториал по их использованию](https://github.com/BobaZooba/DeepNLP/blob/master/Tutorials/Word%20vectors%20%26%20Data%20Loading.ipynb).

Вам предстоит реализовать такую модель:
![Архитектура модели DAN](https://www.researchgate.net/profile/Shervin-Minaee/publication/340523298/figure/fig1/AS:878252264550411@1586403065555/The-architecture-of-the-Deep-Average-Network-DAN-10.ppm)

Что она из себя представляет:
- Мы подаем в нее индексы слов
- Переводим индексы слов в эмбеддинги
- Усредняем эмбеддинги
- Пропускаем усредненные эмбеддинги через `Multilayer Perceptron`

В этой домашке вам предстоит:
- Перевести тексты в матрицы с индексами токенов
- Реализовать модель
- Обучить ее
- Понять хорошо ли вы это сделали

Это очень важная модель, потому что она очень простая и показывает достаточно высокие метрики. В дальнейшем на работе советую использовать такую модель как бейзлайн. И в качестве эмбеддингов слов взять эмбеддинги от берта/роберты/тд.

Используйте слои: `nn.Linear`, `nn.BatchNorm`, `nn.Dropout` и тд.

## Установка зависимостей
Необходимые сторонние библиотеки  
`pip install -r requirements.txt`

## Оценивание
Будет проверяться корректность логики обучения, 
будут даваться комментарии что нужно исправить, 
если домашка будет сдана вовремя. 
Максимальный балл: 10.

## Дедлайн
26/10/2021  
Далее максимальный балл за работу: 7

## Важные просьбы
- Не отправляйте ссылку на `colab`
- Прежде чем отправить задание на проверку, очистите свой код от неиспользоваемого кода и неважных комментариев
