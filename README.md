# Normalize Russian Car Numbers

# Aligning Car License Plate Images

# Customer

![beeline-Photoroom](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/55a73fe2-752d-4888-9d3b-70b01f2b50d2)

Beeline, developed as part of the hackathon **Digital Breakthrough, Season: Artificial Intelligence**

# Problem

- Today, video surveillance for car license plate recognition has become standard practice  
- A key challenge is the quality of plate recognition, especially under poor lighting, various viewing angles, and blurry images  
- An important step in this process is plate alignment to ensure accurate recognition of each character  

![asdfghjklimage](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/3ede15a7-30e6-41f9-9320-0de84b003d30)

![image](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/a1460028-cced-4cad-bdc7-ae16aa8558c5)

# Final Product

A software module that allows calling the license plate alignment algorithm, usable for single images or batches.  

Our algorithm consists of 3 steps:  
1) License plate segmentation  
2) Resize to the required dimensions  
3) Alignment using a template  

![Screenshot_94_3](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/e8836455-c033-40fe-973c-1d495bb05120)

# Technology Stack

- PyTorch  
- OpenCV  
- NumPy  
- pandas  
- Pillow  
- Roboflow  
- Docker

# Key Advantage

## Algorithm Uniqueness

- Our segmentation model for car plates is trained on a custom annotated dataset in Roboflow, using data augmentation for larger volume. The algorithm processes **20 images per second**. Accuracy, measured on our metric, averages **79%**  
- We also use strict mathematical and matrix operations via OpenCV for precise plate alignment, which greatly reduces errors

# Practical Applicability

> Implementing our plate alignment algorithm significantly improves the accuracy and efficiency of video surveillance systems that rely on car plate recognition.  

> This is particularly important for businesses in security, law enforcement, vehicle monitoring, and parking management.

# Scalability

- The algorithm can be adapted for license plates from other countries, not just Russia. This requires retraining the segmentation model on annotated data of foreign plates  
- It can also handle large input streams, provided sufficient computational resources are available

# How to Run the Application

- Instructions can be found in the [src folder](src/)  
- All Jupyter Notebooks used for analysis and model training are in the [notebooks folder](notebooks/)  
- Model weights are available [here](https://drive.google.com/drive/folders/1NFzOVovRzFjN6iBO0q58cqdTAWhHdaTt?usp=drive_link)

# Team

**Egor Andreasyan**  
> ML Engineer  
- Email: egorandreasyan@yandex.ru  
- Telegram: @EgorAndrik  

**Mikhail Vershinin**  
> ML Engineer  
- Email: m_ver08@mail.ru  
- Telegram: @Radsdafar08  

**Semen Suslyakov**  
> BackEnd Developer  
- Email: ssuslyakoff@gmail.com  
- Telegram: @ssuslyakoff  

**Alexander Rotachyov**  
> CV Engineer  
- Email: rotachevaa07@gmail.com  
- Telegram: @developweb3



# Normalize-russian-cars-numbers

# Выравнивание изображений номеров автомобилей

# Заказчик

![beeline-Photoroom](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/55a73fe2-752d-4888-9d3b-70b01f2b50d2)

Beeline, сделанно в рамках хакатона Цифровой Прорыв сезон: Искусственный Интеллект

# Проблематика

- На сегодняшний день использование видеонаблюдения для распознавания номеров автомобилей стало обычной практикой
- Однако ключевая проблема заключается в качестве распознавания номеров, особенно в условиях неблагоприятной освещённости, различных углов обзора и размытости изображений.
- Важным этапом в этом процессе является выравнивание номеров, чтобы обеспечить точность распознавания каждого символа.

![asdfghjklimage](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/3ede15a7-30e6-41f9-9320-0de84b003d30)

![image](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/a1460028-cced-4cad-bdc7-ae16aa8558c5)

# Итоговый продукт

Программный моудль, который можно использовать для обращения к алгоритмувыравнивания номеров, причём можно использовать это как для одной картинки, так и для нескольких сразу.

Наш алгоритм состоит из 3 шагов
1) Сегментация номерного знака
2) Преобразование в нужный размер
3) Выравнивание по трафарету

![Screenshot_94_3](https://github.com/NSO-Clio/Normalize-cars-numbers/assets/124351915/e8836455-c033-40fe-973c-1d495bb05120)


# Stack технологий

- PyTorch
- OpenCV
- NumPy
- pandas
- pillow
- roboflow
- Docker


# Наш главный плюс 

## Уникальность алгоритма

- Наша сегментационная модель для номеров автомобилей на фото обучена на созданном и размеченном нами датасете в roboflow с использованием аугментации для большего объёма данных. Скорость работы алгоритма 20 фото в секунду. Точность модели по собственной метрике показывает относительно неплохой результат – в среднем 79%
- Также мы используем строгие математические и матричные операции через OpenCV для выравнивания номера, что сильно сокращает количество ошибок


# Практическая применимость

> Реализация нашего алгоритма по выравниванию номеров значительно повышает точность и эффективность систем видеонаблюдения, использующих распознавание номеров автомобилей.
 
> Это особенно важно для бизнеса, работающего в сферах безопасности, правоохранительных органов, контроля транспортных средств, управления парковками.


# Масштабируемость

- Наш алгоритм можно использовать для выравнивания номеров и других стран, не только России. Для этого необходимо дообучить сегментационную модель на размеченных данных номеров других стран. 

- Также наш алгоритм можно использовать для большого количества входных потоков данных, при условии увеличения вычислительных ресурсов.


# Как запустить приложение?

- как запустить проект можно посмотреть по ссылке в папке [src](src/)
- В папке [notebooks](notebooks/) указаны все Jupyter Notebook-и в которых проводился анализ и обучения модели
- Веса модели можно посмотреть по ссылке https://drive.google.com/drive/folders/1NFzOVovRzFjN6iBO0q58cqdTAWhHdaTt?usp=drive_link

# Наша команда

**Андреасян Егор**
> ML-инженер
- Почта: egorandreasyan@yandex.ru
- telegram: @EgorAndrik

**Вершинин Михаил**
> ML-инженер
- Почта: m_ver08@mail.ru
- telegram: @Radsdafar08

**Сусляков Семен**
> BackEnd-разработчик
- Почта: ssuslyakoff@gmail.com
- telegram: @ssuslyakoff

**Ротачёв Александр**
> CV-инженер
- email: rotachevaa07@gmail.com
- telegram: @developweb3
