  Порядок ветвления 

Ветки : dev - ветка текущей разработки и изменений, debug - отладка кода без изменений в логике работы ,
master/main - ветка с актуальной и рабочей версией программы, hotfix - ветка с малыми исправлениями в ветке master/main

Последовательность
  Разработка
commit->dev->debug->main
  Внесение срочных малых изменений в актуальную версию
main->hotfix->main
  Пример

        
            debug 
          /          \  
      dev              \
    /                    \
main----------------------main---------main
                              \        /
                                hotfix

Порядок оформления текущей работы
Добавляем issue потом в коммите указываем его.
Важно старатся работать по одному issue за коммит.
В wiki нужно записать текущий функционал с примером кода и работы(если есть возможность). Оформление на усмотрении разработчика.



  Задание

Написать класс для представления парковки с проверкой времени заезда машины и графиком работы самой парковки с 8 до 22

  Открытый функционал (public)
Сколько места (количество в штуках и в процентах)
Приезд машины (попытка вставки)
Уезд машины 
Возможность реализации очереди из машин

  Требования к реализации
Места должны быть определены в куче (динамически) , а не в стеке (статически).Это нужно для расширения парковки, если потребуется.
Класс не должен предоставлять какой-либо вывод внутри себя, для этого нужны будут методы проверок нужных вам состояний (полная, свободная и тд).
Время заезда машины не следует хранить в объектах машины или парковки.


