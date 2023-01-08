# Домашнее задание к занятию "`10.2 Кластеризация`" - `Mashalov V.V.`



### Задание 1
```
Задание 1.
В чем различие между SMP и MPP системами?

Приведите ответ в свободной форме.
```

>Сильно связанная система(SMP) состоит из нескольких однородных
процессоров и общей памяти, когда как в слабо связанных системах(MPP) вся память распределена между процессорными элементами.

---

### Задание 2
```
В чем отличие сильно связанных и слабо связанных систем?

Приведите ответ в свободной форме.
```
> + Степень связи между процессорами в слабосвязанной системе низкая, тогда как степень связи между процессорами в тесно связанной системе высока.
> + Основное различие между слабосвязанной и тесно связанной многопроцессорной системой заключается в том, что слабосвязанная система имеет распределенную память, тогда как тесно связанная система имеет общую память.
> + Слабосвязанные системы обладают более низкими скоростями передачи данных, но в то же время дешевле, когда как сильносвязанные более производительны, при повышенной стоимости.


### Задание 3
```
Какие преимущества отличают кластерные системы от обычных серверов?

Приведите ответ в свободной форме.
```
> + Применение кластера высокой готовности позволяет предотвратить как неплановые простои, вызываемые отказами аппаратуры и программного обеспечения, так и плановые простои, необходимые для обновления программного обеспечения или профилактического ремонта оборудования.
> + У кластерных систем практически безконечная масштабируемость, упирающиеся только во внешние системы (такие как электроснабжение, скорость интернета и пр.)

### Задание 4

```
Приведите примеры типов современных кластерных систем?

Приведите ответ в свободной форме.
```
> + отказоустойчивые кластеры (High-availability clusters, HA,
кластеры высокой доступности);
> + кластеры с балансировкой нагрузки (Load balancing clusters);
> + вычислительные кластеры (High performance computing
clusters, HPC);
> + системы распределенных вычислений.
---


### Задание 5
```
Где использует сервис Kafka, rabitMQ?

Приведите ответ в свободной форме.
```
> + Apache Kafka лучше всего подходит для потоковой передачи от А к Б без сложной маршрутизации, но с максимальной пропускной способностью. Инструмент отлично справляется с event sourcing, потоковой обработкой и моделированием изменений в системе в качестве последовательности событий. Кафку также можно использовать для обработки данных при многоэтапной конвейерной обработке.
>> Кафка станет отличным решением, если вам нужен фреймворк для хранения, чтения, повторного чтения и анализа потоковых данных. Ее сильная сторона – обработка и анализ данных в реальном времени. Инструмент идеально подходит для постоянного хранения сообщений или для регулярно проверяемых систем.
> + Разработчики используют RabbitMQ для обработки высокопроизводительных и надежных фоновых заданий, а также для интеграции и взаимодействия внутри приложений и между ними. Инструмент применяется для выполнения сложной маршрутизации к консьюмерам и интеграции нескольких приложений и служб с нетривиальной логикой маршрутизации.
>>RabbitMQ идеально подходит для веб-серверов, которым требуется быстрый запрос-ответ. Этот инструмент распределяет нагрузку между рабочими приложениями при высокой нагрузке (более 20 000 сообщений в секунду) и может обрабатывать фоновые задания или длительные задачи, такие как преобразование PDF, сканирование файлов или масштабирование изображений.
---