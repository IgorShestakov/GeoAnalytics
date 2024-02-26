# DataSets

Датасет Russia Real Estate 2018-2021 взят с [Kaggle](https://www.kaggle.com/datasets/mrdaniilak/russia-real-estate-20182021) 
Общий объем данных 540 тысяч строк объявлений с сайтов о продаже недвижимости. Особенностью датасеты является некорректный номер региона у данных.

Датасет Russia boundaries geo data взят с [Kaggle](https://www.kaggle.com/datasets/kapral42/russia-geo-data/data) 
Границы регионов РФ представлены на 2015 год.

В рамках данной работы:
- Создан GeoDataFrame с формированием столбца с координатами.
- Использован метод sjoin(Spatial join),с использованием операции within, которая позволяет проверить вхождение точек в полигоны и подтянуть корректное поле регионов для каждой строки.
