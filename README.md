# Цифровой прорыв 2022 | Ульяновская область   
### Задача:
Разработать алгоритм, позволяющий определить дистанцию до впереди идущего автомобиля в режиме реального времени, используя для этого датасет фотографий автомобилей с разного расстояния. 
### Мое решение:
За основу решения был взят baseline предоставленный организаторами чемпионата, который был улучшен, а именно, помимо детектирования машины, детектировался еще номер и автомомбильный значок, что давало больший прирост в скоре. Дополнительные модели были предобучены на train данных соревнования (ручная разметка с помощью онлайн сервиса [makesense.ai](https://www.makesense.ai/)) с использованием модели [YOLOv5](https://github.com/ultralytics/yolov5) (YOLOv5m6). Для предсказания расстояния был использован CatBoostRegressor с улучшенными параметрами.
![image](https://user-images.githubusercontent.com/69726878/186945958-e98fd36c-cbe1-4d0e-b0cd-c7f0af825765.png)
    
  
Мое решение: ```cp.ipynb```  
Детектирование автомобилей, автомобильных номеров: ```car-plate-logo-yolov5.ipynb```  

### Дополнительные ссылки:
[Цифровой прорыв 2022](https://hacks-ai.ru/)  
[Мое видео решение](https://disk.yandex.ru/d/H7LbKCeuhMDI4w)  
[Веса](https://disk.yandex.ru/d/H2A9BQekz75zMw)  
[Вспомогательные Kaggle Notebook для обучения данных с помощью YOLOv5](https://www.kaggle.com/code/gowrishankarp/license-plate-detection-yolov5-pytesseract/notebook)  
[Car Plate Get Annotation Info from XML](https://www.kaggle.com/code/stpeteishii/car-plate-get-annotation-info-from-xml)  

