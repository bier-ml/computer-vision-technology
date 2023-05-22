# Курс Технологии компьютерного зрения

## Описание курса



## Пререквизиты

Основы математики: линейная алгебра, дифференциальные уравнения, теория вероятности и статистика.

Программирование на языках Python: студенты должны уметь писать программы, основанные на алгоритмах компьютерного зрения, а также иметь понимание ООП и использование соответствующих библиотек и фреймворков, таких как NumPy, OpenCV, TensorFlow, PyTorch.

Обработка изображений: студентам следует иметь представление о цифровой обработке изображений, методах фильтрации и улучшения изображений, а также сегментации изображений.

Машинное обучение: студентам необходимо знать основные понятия машинного обучения, методы обучения с учителем и без учителя, а также классификацию и регрессию.

Глубокое обучение: студентам следует иметь понимание основных концепций глубокого обучения, нейронных сетей и сверточных нейронных сетей, а также уметь обучать глубокие нейронные сети.

## Материалы для подготовки к курсу


## Источники
...

## Оценочные средства
...

## Описание технологии проведения итогового экзамена

Оценка за курс ставится исходя из набранных баллов за выполнения практических заданий

## Результаты обучения
Какие навыки студенты прокачают после прохождения курса. С указанием уровня.


## План курса

    1 Tracking. Re-Identification. Sort, DeepSort
    
    2 Object detection and Semantic Segmentation
    
    3 Технологии работы с видео. ffmpeg, gstreamer, deepstream

    4 Pose estimation
    
    5 Optical Character Recognition

    6 Action recognition

    7 Generative ML


## Критерии оценки пройденных тем
### 1 "Tracking. Re-Identification. Sort, DeepSort":
Студенту необходимо реализовать методы tracker_soft, tracker_strong и метод подсчета метрик, а также написать отчет. 
Все подробности тут https://github.com/VABer-dv/object-tracking-assignment

Критерии оценки дз по теме:

Оценка неудовлетворительно (2) ставится, если:
- студент все сделал, но не может рассказать как работает его код и что происходит в проекте
- код полностью заимствован у другой команды/из репозитория
- нарушен оговоренный срок сдачи и защиты дз

Оценка удовлетворительно (3) ставится, если:
- студент реализовал только 1 метод трекера + метод подсчета метрик, при этом презентация самой работы произведена плохо, 
студент с трудом отвечает на вопросы по проекту, отчет по работе не отвечает критериям (проговаривал на лекции)

Оценка хорошо (4) ставится, если:
- студент реализовал только 1 метод трекера + метод подсчета метрик, быстро ориентируется в коде проекта, отвечает на
поставленные вопросы на защите, отчет отвечает критериям

или

- студент реализовал 2 метода трекера + метод подсчета метрик, но имеет сложности в презентации и защите работы, 
нуждается в большом количестве наводящих вопросов, чтобы ответить на первоначальный вопрос, имеет недочеты в оформлении 
отчета

Оценка отлично (5) ставится, если:
- студент сдал и защитил работу в кратчайший срок, на ближайшей официальной практике после лекции; при этом работа может
иметь недочеты или шероховатости, но студент должен хорошо разбираться в презентуемом материале и представленном проекте

или

- студент реализовал 2 метода трекера + метод подсчета метрик, быстро ориентируется в коде проекта, отвечает на 
поставленные вопросы на защите, отчет отвечает критериям
### 2 "Object detection and Semantic Segmentation":
Группе необходимо составить доклад по одной из предложенных к обзору архитектур детектора или сегментатора. Доклад должен содержать описание архитектуры, ее особенности и улучшения по сравнению с дочерними или конкурентными решениями. Также по теме доклада необходимо подготовить выступление и презентацию и защитить его на практическом занятии. Список допустимых к обзору архитектур (специфических задач решений функций ошибок и т.д.) гибкий и тема может быть согласована с ментором индивидуально. Тайминг защиты - 5 минут доклад + 2 минуты ответы на вопросы.

Критерии оценки дз по теме:
- Описание в докладе решаемой проблемы
- Описание в докладе идеи и реализации
- Раскрытие в презентации важных отличительных черт
- Вовлеченность в защиту всех членов команды
- Ответы на вопросы

Оценка выставляется комплексная с учетом пречисленных выше критериев. В случае отсутствия группы на защите итоговая оценка будет снижена на балл.

### 5 "Optical Character Recognition":
Студенту необходимо реализовать архитектуру CRNN из [статьи](https://arxiv.org/abs/1507.05717).
В качестве генератора датасета рекомендуется использовать файл репозитория Topic 5. OCR/dataset.py, однако можно 
написать свой генератор капч или готовый датасет. 

Оценка отлично (5) ставится, если:  

- архитектура реализована точно как описано в статье, а не просто похожа  
- выбрана и обоснована метрика качества  
- модель обучена и запускается в демо режиме - т.е. есть скрипт, который загружает обученную модель, на лету генерируется капча, модель её распознает
- есть понимание работы CTC loss  
- ответы на вопросы  
- студент сдал и защитил работу в кратчайший срок, на ближайшей официальной практике после лекции

Оценка хорошо (4) ставится, если:  

- модель реализована, есть неточности реализации  
- выбрана и обоснована метрика качества  
- модель обучена и запускается в демо режиме  
- есть понимание работы CTC loss  
- ответы на вопросы

Оценка удовлетворительно (3) ставится, если:

- модель реализована, есть неточности реализации
- модель обучена и запускается в демо режиме
- ответы на вопросы

Оценка неудовлетворительно (2) ставится, если:

- код полностью позаимствован из других источников
- модель не запускается
- нет ответов на вопросы

## Команда курса

- [Владимир Фоменко](https://github.com/Vlako)
- [Артур Идятов](https://github.com/electriclizard)
- [Емельян Бурыкин](https://github.com/Emelian)
- [Владислав Бережной](https://github.com/VABer-dv)
- [Александр Бармин]()
- [Евгений Кириллов](https://github.com/Skyfallk)
