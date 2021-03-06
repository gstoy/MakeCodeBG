Работа с блокове от категория Radio
===================================

В този урок ще се запознаем с блоковете от категория |Radio|, напр.блоковете , използвани за установяване на връзка и комуникация с две или повече Micro:bit устройства. В такъв случай няма да използваме Micro:bit-ове, а симулатор, който ще представи двата Micro:bit–а на екран. 
Така всички създадени кодове ще се работят на двата виртуални Micro:bit-а.

.. |Radio| image:: ../_images/_imageMicroBit/s21.png

Създайте програма, която при натискане на бутона А, изпраща случайно число от 0 до 100. Когато тази информация е получена, светлина се появява в средата на екрана, образувайки 3Х3 квадрат, ако полученото число е четно, или посочвайки съответната стойност на числото, ако то е нечетно.

Създавайки ID група, ние всъщностсъздаваме пространство за комуникация между две устройства.

За да създадем ID група, трябва за влачим блока |radioset| от категорията |Radio| в блока |onstart|. В полето за въвеждане на числа и текст можем да впишем желаното число за ID групата, което може да бъде всяко число. Ние ще зададем числото 1. По този начин създадохме ID група 1, където двата Micro:bit-а могат да комуникират.

.. |onstart| image:: ../_images/_imageMicroBit/s20.png

.. |radioset| image:: ../_images/_imageMicroBit/s22.png

.. image:: ../_images/_imageMicroBit/s24.png
      :align: center

Забележка: когато използваме блоковете от категорията ``Radio``,ще има два Micro:bit-а, показани в симулатора.

Променливата ``Counter`` съхранява стойностите, получени чрез употребата на блока |pickrandom|, или казано по друг начин, променливата ``Counter`` получава една случайнна стойност от 0 до 100. 
Когато бутонът А е натиснат, Micro:bit-ът изпраща стойността на променливата ``Counter`` използвайки блока |send| от категория |Radio|.

Блокът изглежда така:

.. |pickrandom| image:: ../_images/_imageMicroBit/p49.png
.. |send| image:: ../_images/_imageMicroBit/s30.png

.. image:: ../_images/_imageMicroBit/p73.png
      :align: center

Когато информацията е изпратена, тя следва да бъде получена. На база на тази информация, изпълнението на програмата се определя (ще се покаже квадратче при четно число или ще се покаже конкретното чесло при нечетно такова). За тази цел ще влачим блок от категорията |Radio| :

.. image:: ../_images/_imageMicroBit/p73.png
      :align: center

В този блок ще влачим блок, който дефинира променливата ``Remainder``, която съхранява стойностите за цялото делене ``Counter`` на 2:

.. image:: ../_images/_imageMicroBit/p64.png
      :align: center

Това е последвано от блока |ifthen|. В частта |uslov|   ще проверим дали има остатък след цялото делене на Брояча на 2. Ако е вярно, 3х3 квадрат ще се появи на екрана. Иначе, условието не би било изпълнено, което означава, че остатъкът не е 0, тогава стойността на променливвата ще се покаже:

.. image:: ../_images/_imageMicroBit/p75.png
      :align: center

.. |ifthen| image:: ../_images/_imageMicroBit/s3.png
.. |uslov| image:: ../_images/_imageMicroBit/s5.png

Крайният вид на кода:

.. image:: ../_images/_imageMicroBit/p76.png
      :align: center

Линка за кода: https://makecode.microbit.org/_f31EfHcv6Kpy

Ще тестваме програмата презз симулатора, натискайки |play|.

.. |play| image:: ../_images/_imageMicroBit/p3.png

.. mchoice:: L8Z1
    :answer_a: Когато данните бъдат получени, нищо няма да се появи.
    :answer_b: Когато данните бъдат получени, LED с координатите (2,2) ще светне.
    :answer_c: Когато данните бъдат получени, съобщението „Здравей“ ще се покаже.
    :feedback_a: Браво!
    :feedback_b: Грешен отговор!
    :feedback_c: Грешен отговор!
    :correct: a

    Изучете блоковете внимателно.

    .. image:: ../_images/_imageMicroBit/p77.png
          :align: center

    Какво ще се покаже след изпълнението на посочените блокове?

**Задача:** Наредете блоковете, така че да симулират операцията на телеграф, по- точно, когато сигнал (число) бъде изпратено, LED-овете да светват в случайникоординати.

**Малко помощ:** Стойностите на координатите х и у са от интервала от 0 до 4.

Сравнете решението си с нашето: https://makecode.microbit.org/_JgFC5vRpudkq
