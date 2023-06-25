# hacks-ai-2023
Выполнено в ходе хакатона 2023 "Цифровой прорыв Сезон:Искусственный интеллект". Кейс - самолет.

## Кейс
Одна из основных статей расходов девелоперов – это закупка материалов. При этом среди общих затрат на материалы около 10% приходится на арматуру. 

Упрощенно процесс закупки материалов выглядит так: 
категорийный менеджер устраивает тендер на закупку арматуры объема Х (для простоты давайте считать, что потребность «Самолета» в арматуре постоянна, компании нужно Х тонн в неделю). Например, он может организовать тендер на объем 5Х или на объем 2Х. Он знает, какая цена на арматуру сегодня, но не знает, какая она будет через неделю. 
В принятии решения о размере проводимого тендера может помочь прогнозная модель. Участникам хакатона предстоит разработать модель прогнозирования цены, что позволит снизить затраты категорийного менеджера при проведении тендеров на закупку.

---

Мы предоставляем решение для вычисления изменения цены на арматуру на N недель вперед. Использовался следующий подход:

на первом шаге мы обработали предоставленный набор данных с ценами на сырье

на втором мы обучили модель на прогнозированию цен полученных данных

на третьем шаге мы, используя вычисленные цены, вычисляем стратегию закупки и анализируем с помощью скользящего среднего значения.

## Стек

Python, pandas, numpy, darts, matplotlib, seaborn.

## Colab

Обучение модели https://colab.research.google.com/drive/1JMZq4ZqvKrWm0jju1NSvST9V2Dw2Cl0W

Использование модели https://drive.google.com/file/d/1EUoU75qYagvu2qKKMKlUsCiEnb5_cXCo/view?usp=sharing

Результат метрики

![image](https://github.com/asdafafs/hacks-ai-2023/assets/75051539/849e1a20-aa83-4710-a20f-ca257073c89c)
