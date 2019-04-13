# Настройка репозитория
Чтобы гарантированно запускать примеры из семинаров с теми же
версиями библиотек, а также запускать задачи из домашнего задания необходимо создать
вирутальное окружение с `python3.6`. 

## Пример настройки с использованием [`virtualenv`](https://virtualenv.pypa.io/en/stable/userguide/)

1. Создайте виртуальное окружение `virtualenv -p python3.6 <path_to_dir_where_env_will_be_stored>`
2. Активируйте  `source <path_to_the_dir/bin/activate>` (для windows: `<path_to_the_dir\Scripts\activate>`), для выхода используйте команду `deactivate` 
3. Установите необходимые пакеты `pip install -r <path_to_rep_requirements.txt>`
Выполнив эту команду, вы получите такую же кофигурацию библиотек, которая используется на семинарах, лекциях и в домашних заданиях.

## Jupyter Notebook
Большую часть кода мы будем писать и изучать в [`jupyter notebook`](https://jupyter.org/install) (нужные пакеты указаны в файле requirements.txt).
Нужно поднять сервер Jupyter Notebook. 

1. Выполните команду `jupyter notebook --port 3040 --port-retries=0 --ip='*' --no-browser`. Теперь вы можете зайти в браузере на страницу [http://localhost:3040/tree](http://localhost:3040/tree) и увидеть проводник. Корневой папкой будет та, находясь в которой, вы выполнили команду запуска.
2. Добавьте в `jupyter notebook` созданное ранее виртуальное окружение как новый `Kernel`.
Находясь в виртуальном окружении выполните команду
`ipython kernel install --user --name=<name_of_kernel>`.  
Теперь вы можете переключиться на нужное ядро через `Kernel` > `Change kernel` прямо в открытом ноутбуке с кодом.

***

# Примерный план занятий

**1. Лекция**
* Flow проектов: какие есть этапы и зачем они нужны
* Роли в ds команде
* Кейс про очереди

**1. Семинар**
* Как организовывать код проектов
* Основы git
* virtualenv и пакеты в питоне

---

**2. Лекция**
* Presale стадия проекта: важные моменты
* Визуализация данных
* Статистический анализ
* Когнитивные искажения и как их обходить
* Базовые понятия map reduce 

**2. Семинар**
* Визуализация данных в питоне на примерах
* Работа с pandas, numpy, scipy при анализе данных
* Пример Map Reduce в Питоне

---

**3. Лекция**
* Градиентный бустинг и бэггинг
* Нюансы обучения и применения на практике
* Кейс про рекомендации к заказу

**3. Семинар**
* Обзор библиотек градиентного бустинга в питоне
* Паттерны при обучении моделей

---

**4. Лекция**
* Линейные модели и Нейронные сети
* Нюансы обучения и применения на практике
* Кейс про оптимизацию рекламного бюджета / проверку автомобилей

**4. Семинар**
* Обзор библиотек для обучения линейных моделей и для нейронных сетей

---

**5. Лекция**
* Тройственность метрик (оффлайн-онлайн-лосс) и как с ней жить
* Общепринятые метрики в разных областях и задачах
* Методы кастомизации моделей под метрики при обучении
* Быстрые кейсы на постановку и выбор метрики

**5. Семинар**
* Реализация кастомных лоссов в разных библиотеках (gb и nn)
* black box optimization

---

**6. Лекция**
* Основные паттерны программирования: фабрика, адаптер, синглтон и другие
* Архитектура сервиса для применения моделей: важные составляющие, взаимодействие, проблемы

**6. Семинар**
* Реализация основных паттернов программирования в питоне 
* Прототипирование задач на питоне
* Реализация ml сервиса на питоне

---

**7. Лекция**
* Оптимизация работы ds кода: извлечение tf матриц, numpy-изация, обёртки над плюсовым кодом
* Кейс про проверку автомобилей / оптимизацию рекламного бюджета

**7. Семинар**
* Основы html+css (и немного javascript)
* Майнинг данных из внешних источников

---

**8. Лекция**
* Основы проверки статистических гипотез и АБ тестирование

**8. Семинар**
* Основы проверки статистических гипотез и АБ тестирование (практика)

---

**9. Резервные темы (также можем расширить по предложению слушателей, пишите [сюда](https://goo.gl/forms/jQsATnKAlvLM1RPf1))**
* Продвинутые паттерны в аб тестировании
* Как проходят собеседования в DS
* Дополнительные кейсы
* Подробнее про Map Reduce
* Как работают базы данных


