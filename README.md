Дана информация о сотрудниках некоторой компании. Необходимо распределить премию между сотрудниками по результатм успехов. Для анализа по каждой должности есть свой HR-менеджер, который сравнивает сотрудников друг с другом внутри одной должности.
### Необходимо разработать дашборд, который будет решать следующие задачи:
1. Основная метрика для оценки сотрудников – performance rating (далее рейтинг), он может принимать значения от 1 до 4. 1 — плохая работа, 2 — в рамках ожиданий, 3 — выше ожиданий, 4 — превосходные результаты. По рейтингу вы определяете уровень, какой % от зарплаты будет выдан в качестве дополнительной премии. Если рейтинг сотрудника ниже среднего по его должности, то он получает 5-10%-ную премию от годового дохода, если выше среднего, то 10-20%. Сотрудники с рейтингом 1 не премируются, им предлагается бесплатное корпоративное обучение, которые может помочь им повысить свой перфоманс результат. Для точного определения процентов внутри диапазона используется анализ количества закрытых проектов за рабочий период (projects closed). Сотрудники выполнившие более 15 проектов получают 8-10% при перфоманс рейтинга ниже среднего и 15-20% при выше среднего. Проекты примерно равнозначны среди должностей, поэтому такое сравнение валидно.   
2. Если проектов более 15 и рейтинг выше среднего, то процент уже 15-20%, а если менее 15 и рейтинг выше среднего, то 10-15%. Если проектов более 15 и рейтинг ниже среднего, то процент уже 8-10%, а если менее 15 и рейтинг ниже среднего, то 5-8%.   
3. Финальные значения процентов определяет HR-менеджер индивидуально для каждого сотрудника. Поэтому для принятия решения о премии также во внимание берется самооценка сотрудником удовлетворенности работой, стаж работы и уровень зарплаты. Точно алгоритма определения нет, каждый HR-менеджер принимает решение сам.   
4. Как руководитель, вы хотите понимать общее распределение рейтинга, количество людей с оценками меньше или больше среднего и их уровень заработной платы, чтобы оценить, скольким какая премия достанется. Чтобы в целом оценивать перфоманс сотрудников нужно некоторые овервью по количеству закрытых проектов по департамента и должностям. Ещё вам важно спрогнозировать бюджет на следующий год, поэтому важно посчитать общую сумму премии за текущий период по максимально возможной процентной ставке по правилам выше. Необходимо сделать калькулятор расчета бюджета премий при изменении границ премий в процентах.     
5. Для менеджеров нужна детальная статистика по сотрудникам: их рейтинг, больше он или меньше среднего по должности, количество закрытых проектов, уровень удовлетворенности работой и зарплата. Менеджеры выкачивают детальную таблицу по своей профессии с предлагаемым процентом премии, а потом корректируют её в ручную в экселе и загружают результаты в систему выплат.   
6. Этим дашбордом будут пользоваться руководитель финансового департамента и его подчиненные раз в квартал на компьютерах. Сейчас эта задача решается через аналитиков – они выгружают Эксель с показателями по сотрудникам и дальше фильтруют и ищут людей для премирования. Это занимает много времени и не все сотрудники быстро умеют строить сводные таблицы и графики.

### Данные находятся в файле Hr data_monetary. Разработанные дашборд доступен по ссылке https://public.tableau.com/app/profile/gareeva.marina/viz/Lesson_3_Gareeva_Monetary/sheet15?publish=yes

### Описание данных:
Name	Description
Age	Возраст
BusinessTravel	Категория частоты бизнес-поездок (часто или не часто ездит)
Department	Департамент, в котором числится работник
DistanceFromHome	Расстояние между домом и офисом в километрах
EducationField	Область образования
EmployeeCount	Колонка для расчета суммарного количества работников
EmployeeNumber	ID работника
Gender	Пол (мужской, женский)
PerformanceRating	Оценка работы сотрудника (1-4, где 4 - превосходный результат)
JobRole	Должность
JobSatisfaction	Уровень удовлетворенности работой (1-4, где 4 - очень удовлетворен)
MaritalStatus	Семейное положение
MonthlyIncome	Месячный доход
NumCompaniesWorked	Количество компаний, в которых до этого работал сотрудник
ProjectsClosed	Количество закрытых проектов за год
TotalWorkingYears	Общий стаж работу в количестве лет
TrainingTimesLastYear	Количество часов повышения квалификации в прошлом году
WorkLifeBalance	Уровень удовлетворенности соотношением работы и личной жизни (1-4, где 4 - отличный баланс)
YearsAtCompany	Количество лет в компании
YearsInCurrentRole	Количество лет в текущей должности
YearsSinceLastPromotion	Количество лет с даты последнего повышения
YearsWithCurrManager	Количество лет вместе с текущим менеджером

![Премии сотрудников](https://user-images.githubusercontent.com/104904113/201986698-6ee8507a-4338-42da-ab45-3a4f45c8fd25.jpg)

