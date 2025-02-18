Целью данного исследования является создание модели для прогноза снижения покупательской активности в ближайшие три месяца и разработать персонализированные предложения для сегментов покупателей.

Перед тем, как начать исследование нам будет необходимо провести предобработку данных. Для начала мы прочитаем все датасеты и проверим названия столбцов и тип данных. Мы проведем поиск пропусков, явных и неявных дубликатов и аномалий.

Далее мы проведем исследовательский анализ данных и визуализируем все признаки, которые описывают поведение на сайте, коммуникации с клиентом, финансовое и продуктовое поведение. Мы выясним, сколько процентов пользователей имеют прежний уровень покупательской активности, сколько в среднем они проводят минут на сайте, сколько просматривают страниц, категорий, какая самая популярная категория и какую выручку суммарно приносят клиенты.

Мы объединим три датасета и разделим выручку и минуты на сайте по каждому периоду. Благодаря этому, мы узнаем разницу в выручке между препредыдущим, предыдущим и текущем месяце, а также выделим самый прибыльный месяц.

Следующим нашим шагом будет корреляционный анализ признаков в датасете. Мы изучим взаимосвязь между признаками и рассчитаем коэффициенты корреляции. Мы изучим мультиколлинеарность между входными признаками. Мы построим диаграммы рассеивания для всех входных признаков и целевого признака покупательская активность. В конце анализа мы опишем связь между входными и целевым признаками.

Для поиска лучшей модели, которая сможет прогнозировать покупательскую активность, мы будем использовать пайплайн. С помощью него мы закодируем количественные и категориальные признаки, и обучим наши тренировочные данные на нескольких моделях. С помощью RandomizedSearchCV мы переберем все модели и их гиперпараметры, и найдем модель с лучшей roc_auc метрикой. 

Дальнейшим шагом будет оценка важности признаков с помощью графиков SHAP: мы найдем самые значимые и нерелевантные признаки, которые влияют на прогноз покупательской активности.

Далее мы проведем сегментацию покупателей, выделим группу клиентов, проанализируем ее признаки и разработаем персонализированные предложения для того, чтобы у этой группы не снижалась покупательская активность. 

В конце исследования благодаря нашей модели и сегментации мы сделаем вывод о том, какие признаки больше всего влияют на уровень покупательской активности.