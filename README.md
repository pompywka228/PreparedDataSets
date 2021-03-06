# PreparedDataSets
Подготовленные наборы данных для курсовых работ

# Набор №1 - "Музеи России".
Источник: https://opendata.mkrf.ru/opendata/7705851331-stat_museum  
Данные о музеях России: размер коллекции, график работы и т.п.

Структура:  
name			-	Название музея  
base_fond		-	Число предметов основного фонда на конец года  
science_fond	-	Число предметов научно-вспомогательного фонда на конец года  
ams				-	Автоматизированная музейная система: число внесенных музейных предметов  
n_buildings		-	Число строений  
n_days			-	Число дней в году, открытых для посещения  
guests			-	Число посещений выставок, экспозиций + экскурсионных посещений, тысяч человек  
employees		-	Численность работников, человек  

Задача: вычисление значения параметра guests на основании остальных параметров.  

# Набор №2 "Цены квартир в Москве"
https://www.kaggle.com/hugoncosta/price-of-flats-in-moscow  
Данные о стоимости квартир в Москве в зависимости от параметров квартиры и ее расположения.

Структура:  
price			-	Цена квартиры в $1000  
totsp			-	Общая площадь квартиры, кв.м.  
livesp			-	Жилая площадь квартиры, кв.м.  
kitsp			-	Площадь кухни, кв.м.  
dist			-	Расстояние от центра в км.  
metrdist		-	Расстояние до метро в минутах  
walk			-	1 –	пешком от метро, 0 – на транспорте  
brick			-	1 – кирпичный, монолит ж/б, 0 – другой  
floor			-	1 – этаж кроме первого и последнего, 0 – иначе  
code			-	Число от 1 до 8, при помощи которого мы группируем наблюдения по подвыборкам:  
						1. Наблюдения сгруппированы на севере, вокруг 	Калужско-Рижской линии метрополитена  
						2. Север, вокруг Серпуховско-Тимирязевской линии метрополитена  
						3. Северо-запад, вокруг Замоскворецкой линии метрополитена  
						4. Северо-запад, вокруг Таганско-Краснопресненской линии метрополитена  
						5. Юго-восток, вокруг Люблинской линии метрополитена  
						6. Юго-восток, вокруг Таганско-Краснопресненской линии метрополитена  
						7. Восток, вокруг Калиниской линии метрополитена  
						8. Восток, вокруг Арбатско-Покровской линии метрополитена  

Задача: вычисление значения параметра price на основании остальных параметров.  
Опциональный вариант: вычисление значения параметра code на основании остальных параметров.

# Набор №3 "Страны мира"
https://www.kaggle.com/fernandol/countries-of-the-world  
Статистическая информация о странах мира.

Структура:  
country				-	Страна  
region				-	Регион  
population			-	Население  
area				-	Площадь  
coastline			-	Отношение длины побережья к площади  
infant_mortality	-	Детская смертность (на 1000 рождений)  
gdp					-	ВВП на душу населения  
literacy			-	Грамотность  
phones				-	Количество сотовых телефонов на 1000 человек  
arable				-	Процент территории, используемой под сельское хозяйство  
birthrate			-	Рождаемость  
deathrate			-	Смертность  

Задача: вычисление значения параметра population на основании остальных параметров.  
Опциональный вариант: вычисление значения параметра region на основании остальных параметров.

# Набор №4 "Болезни сердца"
https://archive.ics.uci.edu/ml/datasets/Heart+Disease  
Измерение параметров состояния человека при болезни сердца.

Структура:  
age			-	Возраст  
sex			-	Пол: 0 - женский, 1 - мужской  
cp			-	Тип грудной боли: 1 - типичная ангинальная, 2 - атипичная ангинальная, 3 - неангинальная, 4 - безсимптомная  
trestbps	-	Кровяное давление  
chol		-	Концентрация холестерола  
fbs			-	Уровень сахара в крови  
restecg		-	Результат кардиограммы: 0 - нормальный, 1 - ST-T аномалия, 2 - гипертрофия левого желудочка  
thalach		-	Максимальный пульс  
exang		-	Боль вызвана физическими упражнениями: 0 - нет, 1 - да  
oldpeak		-	Уменьшение ST-сегмента после физических упражнений  
slope		-	Форма ST-сегмента после физических упражнений: 1 - наклон вверх, 2 - плоский, 3 - наклон вниз  
ca			-	Количество окрашенных крупных сосудов при флюороскопии  
num			-	Диагноз стеноза артерии: 0 - сужение диаметра менее 50%, 1 - сужение диаметра более 50%  

Задача: вычисление значения параметра age на основании остальных параметров.  
Опциональный вариант: вычисление значения параметра num на основании остальных параметров.

# Набор №5 "Токсичность воды"
https://archive.ics.uci.edu/ml/datasets/QSAR+aquatic+toxicity  
Информация о структуре молекулы вещества и его токсичности для определенного вида рыб.

Структура:  
tpsa		-	Площадь поверхности молекулы, с атомами, которые могут соединяться с фосфором и серой  
saacc		-	Площадь поверхности молекулы, с атомами, которые могут соединяться с водородом  
h-050		-	Количество атомов, которые могут соединяться с водородом  
mlogp		-	Коэффициент липофильноси (стремления модекулы соединяться с ограническими веществами)  
rdchi		-	Топологический коэффициент (определяет форму молекулы)  
gats1p		-	Коэффициент поляризуемости молекулы  
nn			-	Количество атомов азота  
c-040		-	Количество атомов углерода в определенных связях  
lc50		-	Концентрация, при которой погибает более 50% рыб  

Задача: вычисление значения параметра lc50 на основании остальных параметров.  