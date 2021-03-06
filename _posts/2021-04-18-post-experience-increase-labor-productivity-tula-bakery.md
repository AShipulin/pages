---
title: "Опыт повышения производительности труда на Тульском хлебокомбинате"
date: 2021-04-18
toc: true
categories:
  - Статья
tags:
  - производительность
---

# Аннотация

В статье рассматривается опыт повышения производительности труда на предприятии с коротким производственным циклом с использованием имитационной модели на участке логистики готовой продукции. Выявлены причины невыполнения плана отгрузки, разработанного аналитическим способом. В статье приводятся результаты исследования связи тактов производства с отгрузкой, встречающихся на участке экспедиции, особенности определения “узких мест”. Приводятся возможности применения имитационной системы для апробации принимаемых решений.

# Актуальность

В последнее время наблюдается возрастающая потребность производственных и логистических предприятий в оптимизации своих процессов. Повышение производительности труда становится не просто идеей, а необходимым инструментом повышения эффективности для обеспечения стратегии роста предприятия. Существует множество подходов, направленных на повышение производительности труда, например, 5С, PDCA, SMED. Продолжительность процессов нормируется технологическими картами. Производительность на каждом переделе определяется с использованием аналитических формул. Необходимый объем производства рассчитывается в ERP системах автоматически. Планирование производства и сбыта производится без учета взаимного влияния, транспорт считается неограниченным ресурсом. В результате возникают задержки на этапе отгрузки и доставки продукции, которые влияют на удовлетворенность потребителя.

Усложнение технологической и конкурентной ситуации привело к появлению концепции менеджмента, ориентированного на рынок. Зрелость и насыщение рынков заставляют переносить ключевые компетенции с бизнес-процессов продаж и производства на процессы логистики и сервисного обслуживания. Повышение производительности подсистемы логистики готовой продукции, взаимосвязь с производственной подсистемой влияет на улучшение качества работы предприятия в целом.

Индивидуальный характер оказания транспортно-логистических услуг, необходимость оперативного реагирования на потребности рынка обуславливают широкий разброс в формировании ассортимента услуг как по набору, так и по географическому охвату. Реализация услуг характеризуется широким разбросом в операционных циклах и потребных ресурсах. Для оценки производительности необходимо выбрать метод, позволяющий оперировать процессами с различными операционными циклами.

В статье рассматривается построение и исследование имитационной модели подразделения логистики готовой продукции одного из предприятий хлебобулочного производства.

# Методы

Традиционный подход к планированию производства базируется на аналитическом методе. Расчет производительности труда аналитическим методом основывается на определении объема затраченной работы в единицу времени. Для учета конкретной специфики предприятия используют различные поправочные коэффициенты. Сложные взаимосвязи отображаются с использованием принципов системной динамики.

Часто выбор метода определяется учетной системой, используемой на предприятии. Возможности ERP систем по планированию производства построены на теории системных ограничений - ТоС (Theory of Constraints). В основе теории лежит выбор ключевого рабочего центра и его максимально эффективного использования. Методика разработана по принципу «тянущей» системы. В ней используется правило «Барабан-буфер-веревка». Барабаном является ключевой рабочий центр, веревка - обратная связь, а буфер — это страховой запас для обеспечения бесперебойной работы. На каждом этапе производства выделяется «узкое место», удельная производительность которого задает обобщенное время выполнения заказов. В отдельных случаях для получения исходных значений используется аппроксимация функции статистических данных с применением Microsoft Excel или Mathcad. Очевидное преимущество этого метода - скорость и простота расчета за счет очень высокого уровня абстракции. Недостатком является отсутствие отображения управления и взаимного влияния подразделений друг на друга. Более точным методом является графоаналитический метод, но применяется он редко, так как является трудоемким.

Имитационное моделирование — это простой инструмент анализа, так как модели наглядны, просты для понимания и повторяют сложившуюся ментальную модель о системе. С помощью имитационного моделирования находят “узкие места” и дают ясное представление о сложных системах. Имитационную модель можно анализировать в динамике и наблюдать за эмерджентными свойствами системы.

Существует множество имитационных систем, в которых возможно создать имитационную модель, например, популярная AnyLogic. Недостатком имитационных систем является то, что нужен аналитик, который может построить модель. Кроме того, большинство систем являются платными. В исследовании предприятия хлебобулочного производства выбор был сделан в пользу известной и хорошо зарекомендовавшей себя имитационной системы ИСТРА.

Имитационная система ИСТРА ранее применялась для расчета транспортных объектов, в том числе для железнодорожных станций, узлов, морских портов. Развитие системы сегодня позволяет строить макромодели, включающие целые полигоны. Имитационная система ИСТРА сочетает в себе дискретно-событийный метод с учетом структуры элементов системы и управления. Структура имитационной системы ИСТРА представляет собой упорядоченную тройку множества элементов, операций и оператора управления. Операции являются элементарной, «естественной» частью технологического процесса, что позволяет без сложных преобразований достаточно легко и полно моделировать транспортные процессы. В модели реализован ситуационный принцип управления, так как он больше соответствует процессам управления в сложных транспортных системах.

# Результаты

## Исследование объекта

Расчеты аналитическим методом пропускной способности зоны логистики готовой продукции позволяли утверждать, что предприятие должно справляться с объемом производства и сроками отгрузки. На практике происходили отклонения от плана отгрузки. Производительность этого участка становилась ограничением для роста выпуска продукции.

В процессе, протекающем в зоне логистики, задействовано несколько участников

- Комплектовщик - Сотрудник, выполняющий операции по подбору готовой продукции на машину в зоне экспедиции
- Водитель - Сотрудник, выполняющий погрузку товара, в том числе комплектацию по точкам доставки в машину и доставку до клиентов
- Грузчик - Сотрудник, осуществляющий вспомогательные операции и возврат порожних тележек на производство

Процесс предварительной комплектации машины продукцией на участке представлен на рисунке 1.

![](../../assets/images/post-2021-04-18-tula-bakery/2.png)

Рисунок 1. Процесс комплектации машины продукцией

К расчетному времени прибывает машина. Водитель получает документы и выполняет погрузку и окончательную комплектацию с учетом точек доставки по маршруту, рисунок 1.

![](../../assets/images/post-2021-04-18-tula-bakery/2.png)

Рисунок 2. Процесс комплектации с учетом точек доставки по маршруту

Особенностью предприятия является наличие двух участков комплектации, расположенных в шести километрах на удалении друг от друга. Вызвано это наличием второго производства. Ассортимент доставки включает продукцию первого и второго производства. В одном маршруте ассортимент продукции может достигать 78 позиций номенклатуры. На первом производстве ассортимент составляет 49 позиций. На втором производстве ассортимент содержит 66 позиций.

В целях анализа выпускаемой продукции по данными предприятия разработали отчет в Microsoft Power BI, наглядно показывающий плотность потока и структуру.

<iframe width="1140" height="541.25" src="https://app.powerbi.com/reportEmbed?reportId=93714e20-0307-4f68-898f-fbf3abe0f622&autoAuth=true&ctid=1d942a7d-859b-4d5e-85e2-7c2e3b819fe5&config=eyJjbHVzdGVyVXJsIjoiaHR0cHM6Ly93YWJpLXdlc3QtZXVyb3BlLXJlZGlyZWN0LmFuYWx5c2lzLndpbmRvd3MubmV0LyJ9" frameborder="0" allowFullScreen="true"></iframe>

Для доставки продукции используется собственный транспорт, который дислоцируется на первом производстве. В результате отгрузка начинается на первом производстве и состоит из нескольких этапов, показанных на
рисунке 3.

![](../../assets/images/post-2021-04-18-tula-bakery/3.png)

Рисунок 3. Процесс отгрузки на Хлебокомбинате

Наблюдения на участках логистики готовой продукции показали, что затруднения возникли на участке экспедиции второго производства. Вызвано это тем, что машины прибывают с отклонениями от сроков и попадают в очередь. Логистический участок второго производства загружает 111 транспортных средств. Доставка осуществляется в утренние часы, поэтому основная отгрузка выполняется ночью. Плотность прибытия машин для отгрузки для доставки точно в срок представлена на рисунке 4.

![](../../assets/images/post-2021-04-18-tula-bakery/4.png)

Рисунок 4. Плотность прибытия машин для отгрузки
в зону логистики готовой продукции второго производства

При планировании используется технологическая карта комплектации. Суммарное время составляет 11 минут, а время на комплектацию занимает 7 минут на машину.

![](../../assets/images/post-2021-04-18-tula-bakery/5.png)

Рисунок 5. Технологическая карта комплектации по маршруту

Технологическая карта комплектации по маршруту с учетом точек доставки имеет суммарную продолжительность 30 минут, а комплектация составляет 20 минут.

![](../../assets/images/post-2021-04-18-tula-bakery/6.png)

Рисунок 6. Технологическая карта комплектации по маршруту

При натурном наблюдении за процессом были проведены замеры продолжительности выполнения операций. В большинстве случаев комплектация проходила быстрее. Ограничения, выявленные на участке экспедиции:
- прибытие машин имеет стохастический характер;
- одни ворота въезда и выезда с постом охраны, есть задержки;
- стоянка для машин в ожидании в очереди не ограничена;
- одновременная погрузка не более 7 машин, так как 7 ворот;
одновременное размещение в зоне экспедиции не более 4 комплектов доставки, так как площадь - участка экспедиции ограничена;
- один коридор для перемещения груженых и порожних тележек, есть задержки в ожидании  освобождения прохода;
- отсутствует финансирование на техническую модернизацию.

Фактически план отгрузки не выполняется на участке экспедиции и возникает очередь из машин. Задержки длятся до 8 утра.
Анализ причин задержек
Анализ причин задержек на участке логистики готовой продукции экспедиции выявил потери, таблица 2.

Таблица 2. Потери на участке логистики готовой продукции экспедиции

| Вид потерь | Причина |
| --- | --- |
| Ожидание | Встречное передвижение порожних или груженых тележек из-за узкого коридора |
| | Очереди из машин на погрузку из-за отсутствия свободных ворот |
| Транспортировка | Выпадение продукции из лотков на пол в результате перемещений |
| Обработка | Ошибки в комплектации продукции |
| | Повторный пересчет продукции при комплектации из-за некомплектности в лотках
| Издержки | Повторный пересчет продукции при погрузке из-за необходимости распределения продукции по точкам доставки |
| Ненужные действия | Поиск готовой продукции из-за нечеткого закрепления мест размещения продукции и отсутствия ее в зоне экспедиции по причине несвоевременного перемещения |
| | Поиск свободной тары для комплектации машины продукцией|

Наличие различных факторов, снижающих производительность труда, не позволило установить ключевую причину невыполнения плана. Поэтому было принято решение подробно исследовать процессы участка логистики готовой продукции с использованием имитационной системы ИСТРА.

Разработка имитационной модели участка экспедиции
В имитационной системе ИСТРА была построена абстрактная структура участка экспедиции, рисунок 7. В нее вошла стоянка машин, 7 фронтов погрузки, площадь зоны на четыре комплекта.

![](../../assets/images/post-2021-04-18-tula-bakery/7.png)

Рисунок 7. Абстрактная структура логистического участка в имитационной системе ИСТРА
Задана технология выполнения операций по комплектации и погрузке машины, рисунок 8.

![](../../assets/images/post-2021-04-18-tula-bakery/8.png)

Рисунок 8. Технология выполнения операций
в имитационной системе ИСТРА

Продолжительность операции соответствует технологическим картам.

## Верификация имитационной модели

Расчет с использованием фиксированных технологических нормативов показал, что модель не соответствует реальности, очередь из прибывающих машин сохраняется до 10 часов утра. Причина несоответствия в том, что длительность операций в технологических картах отличается от фактической. При установлении норматива не учитывалась ассортиментная линейка продукции. Время на комплектацию машины зависело от ассортимента в маршруте доставки. С учетом фактических, измеренных показателей была скорректирована имитационная модель. Важно отметить, что для расчета на имитационной модели выполняется множество экспериментов. Это обусловлено тем, что модель стала стохастическая и только серия экспериментов может показать устойчивое состояние системы. Время выполнения комплектации по машине лежит в интервале нормального распределения v(3<4<7), комплектация по маршруту с учетом точек доставки в интервале r(10<12<20).

По результатам второй серии экспериментов задержки на участке комплектации снизились, очередь ожидания погрузки сократилась и стала совпадать с реальной ситуацией, рисунок 9. Желтым цветом показана продолжительность ожидания в очереди из машин до 8 часов утра.

![](../../assets/images/post-2021-04-18-tula-bakery/9.png)

Рисунок 9. Очередь из машин в ожидании отгрузки “как есть”

## Апробация управленческих решений

Анализ причин задержек в имитационной модели показал чувствительность модели к несогласованной подаче автомобилей в зону комплектации. Для устойчивой работы системы необходима уравновешивающая (балансирующая) обратная связь, которая бы обеспечивала согласованную комплектацию к моменту прибытия машины.
В результате отгрузка должна быть объединена общим параметром - временем прибытия машин. Фактически это означает начало комплектации под машину после ее выезда с первого производства. Новый процесс отгрузки показан на рисунке 10.

![](../../assets/images/post-2021-04-18-tula-bakery/10.png)

Рисунок 10. Процесс отгрузки в логистической зоне

Изменение только одного параметра показывает, что задержки сократились на час и уменьшилась длина очереди, рисунок 11.

![](../../assets/images/post-2021-04-18-tula-bakery/11.png)

Рисунок 11. Очередь из машин в ожидании отгрузки при согласованных ритмах

Организационные мероприятия, позволяющие снизить потери на участке логистики, представлены в таблице 3.

Таблица 3. Мероприятия по снижению потерь на участке логистики

| Мероприятие | Эффект | Операция |
| - | - | - |
| Размещение постеров с ассортиментом на участке комплектации и указанием количества продукции в лотке | Сокращение времени на подсчет продукции и уменьшение случаев брака | Комплектация по машине |
| Применение правил для лотков, когда в лоток размещается красный флажок, сигнализирующий о несоответствии количества | Сокращение времени на повторный пересчет продукции | Комплектация по машине |
| Использование правил для тележек, когда в одной тележке существует дополнительный пустой лоток, используемый для комплектации продукции | Сокращение времени на поиск пустого лотка | Комплектация по машине |
| Применение правила для тележек, когда используются магниты для крепления листов комплектации, заметок и хранения флажков и маркеров | Сокращение времени на сверку информации по документам | Комплектация - по машине / по маршруту |
| Обеспечение на участке экспедиции своевременного пополнения продукции для комплектования машин | Сокращение времени на поиск продукции и ожидания начала комплектации | Комплектация по машине |
| Исключение встречных перемещений, в том числе возврата используемой тары, тележек в зону погрузки, внесение изменения в маршрут | Исключение ожидания из-за встречного переката тележек по одному коридору | Комплектация - по машине / по маршруту |

Экспертная оценка внедрения указанных мероприятий показала, что сократится время операций комплектации в интервале нормального распределения: по машине  v(3<4<6), по маршруту  r(3<3<18). На основе этих параметров проведена следующая серия экспериментов на имитационной модели. Зона логистики готовой продукции стала устойчива к отклонениям, очередь из машин сократилась, но задержки все еще присутствуют до 7 утра, рисунок 12.

![](../../assets/images/post-2021-04-18-tula-bakery/12.png)

Рисунок 12. Очередь из машин в ожидании отгрузки при внедрении мероприятий

На следующем этапе попытались найти такие параметры участка логистики, когда возможно увеличить объем производства на 30%, используя существующий штат сотрудников.  

Эксперименты на имитационной модели показали, что зона логистики справится с увеличением объема производства на 30% при скорости комплектации по машине v(3<3<6) и комплектации по маршруту r(10<10<15). При этом очереди не будет, а задержки будут минимальными как показано на рисунке 13.

![](../../assets/images/post-2021-04-18-tula-bakery/13.png)

Рисунок 13. Очередь из машин в ожидании отгрузки отсутствует
при увеличении объема отгрузки на 30%

## Обсуждение

На исследуемом предприятии существовал опыт внедрения системы оптимизации маршрутов доставки. Проект завершился неудачей из-за того, что в оптимизационную задачу не смогли заложить все ограничения. Компетенции менеджеров предприятия не позволяют отличать принципы построения имитационной модели и решения оптимизационной задачи. Необходимо доносить мысль, что если процесс можно описать словами, то можно смоделировать его в имитационной системе.

Ограничением по использованию имитационного моделирования на предприятиях является трудоемкость. Разработка модели - это специфическая, творческая задача и напрямую зависит от опыта аналитика. Как правило, аналитиков по построению имитационной модели в штате предприятия нет. Рынок аналитиков ограничивается школами и разработанными ими имитационными системами. Каждая школа имеет специфику по созданию имитационных моделей. Разработка единой нотации языка моделирования и принятие его основными школами способствовали бы более широкому распространению имитационного моделирования.

Как можно доверять результатам имитационного моделирования?
Вовлеченность менеджеров предприятия в процесс написания модели и ее верификации является единственным способом изменения ментального представления. Важно, чтобы на этапе верификации модели были сделаны эксперименты, закономерность которых понятна менеджерам.

Построенная имитационная модель позволяет найти “узкие места“. Практика имитационного моделирования утверждает, что не всегда самый загруженный элемент структуры или технологии является ограничивающим. Самый загруженный элемент структуры - парковка, при этом ее ресурс не ограничен. Причинами задержек на ней являются погрузка, операции по комплектованию и ограниченное место под собранные комплекты. Действительно “узким местом” является скорость комплектации.

Имитационная модель подтвердила, что согласованные ритмы комплектации и прибытия транспорта могут сократить очередь из машин. Это подтверждает важность наличия диспетчерского управления процессами. Полученные результаты позволяют утверждать, что участок экспедиции может справляться с большими объемами производства при организации рациональной работы комплектовщиков.

## Вывод

Планирование производства и доставки готовой продукции с использованием линейных и аналитических методов может приводить к ошибкам. Аналитические методы рассматривают систему не всецело, а частями. С помощью линейных методов невозможно учесть стохастические процессы. Аналитические методы не позволяют определить поведение системы в динамике, когда ритмы тактов процессов не совпадают.

Использование имитационной модели позволяет реализовать синтез аналитического и экспертного метода, воспроизвести эмерджентные связи и системные свойства. С помощью имитационной системы возможно найти барьеры производительности и правильно расставить приоритеты, апробировать управленческие решения.
