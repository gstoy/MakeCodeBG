Работа с блокове от категорията Math and Variables
===========================================================

MakeCode подкрепя четири основни аритметични операции:
- събиране ( + ),
- изваждане ( - ),
- умножение ( * ) и
- деление ( / ).

Блоковете, които активират изчислението се наричат аритметични оператори. Те се намират в категорията |Math|.

.. |Math| image:: ../_images/_imageMicroBit/p41.png

Аритметичните оператори посочват **ЧИСЛО** (като резултат от аритметичната операция).

.. image:: ../_images/_imageMicroBit/p40.png
      :align: center

Резултатът, посочен от аритметичния оператор, може да бъде използван като входяща стойност за блоковете, които приемат числа. Това може да бъде ясно видяно във фигурата горе. Блокът show number …  приема число като входяща стойност и го посочва на екрана.

Представяме ви по-сложен аритметичен израз: ( 2 + 1 ) * ( 12 - 10 ). В MakeCode изчислението би изглеждало така: 

.. image:: ../_images/_imageMicroBit/p42.png
      :align: center

Анализирайки сложния израз, можем да заключим, че той се състои от по-малки части-временни резултати.

Един от тях е (2 + 1). Разликата (12-10) е втория временен резултат. Ще получим крайния резултат от целия израз, когато умножим сумата по разликата (sum * difference).

При програмирането е удобно да се използват междинните резултати (междинни стойности), които наричаме **променливи**. Можете да мислите за променливи като пространства в компютърната памет, подобно на кутии, в които се съхраняват междинните резултати. Променливите имат имена.

Когато искаме да използваме специфична променлива в програмата, достатъчно е просто да посочим найното име.

В MakeCode можем да създадем променливи в категорията |Variables|.

.. |Variables| image:: ../_images/_imageMicroBit/p43.png

Създаваме променливи натискайки бутона Make a variable button (2) в категорията Variable (1), въвеждайки името на променливата (3), която в нашия случай носи името Брояч, и после клекваме на бутона ОК (4).

.. image:: ../_images/_imageMicroBit/11.png
      :align: center

Изразът (2 + 1) * (12 - 10) може да бъде представен и по различен начин- създавайки две променливи: |Zbir| и |Razlika|.

.. |Zbir| image:: ../_images/_imageMicroBit/p45.png

.. |Razlika| image:: ../_images/_imageMicroBit/p44.png

Ще зададем начална стойност 0 на променливата ``Counter``. Това може да стане като влачим блока |set| от категория |Variables| в блока |onstart|.

.. |onstart| image:: ../_images/_imageMicroBit/s20.png

.. |set| image:: ../_images/_imageMicroBit/p47.png

Накрая кодът изглежда така: 

.. image:: ../_images/_imageMicroBit/p46.png
      :align: center

.. mchoice:: L5Z1
    :answer_a: 2.
    :answer_b: 10.
    :answer_c: 4.
    :feedback_a: Браво!
    :feedback_b: Грешен отговор!
    :feedback_c: Грешен отговор!
    :correct: a

    Съдайте програма с две промеливи-х и у. Зададената стойност на х трябва да бъде 2 (x = 2), а на у трябва да бъде 4 (y = 4). 
    Когато програмата прочете блока, показан на фигурата отдолу, резултатът ще бъде: 

    .. image:: ../_images/_imageMicroBit/p48.png
          :align: center


Нека използваме аритметични операции и промеливи, за да създадем програма, която изчислява периметъра и площта на квадрат.

За да изчислим площта на квадрат, трябва да определим дължината на страната ``a``, чиято стойност ще се сменя на случаен принцип всеки път щом потребителят натисне бутона ``A`` , а когато бутонът ``B`` бъде натиснат, програмата ще изчисли периметъра и площта на дадения квадрат.

В самото начало трябва да създадем променливите ``a``, ``P`` и ``A`` , които ще представят съответно страната, периметъра и площта на квадрата.

Случайната смяна на стойностите на променливите ще се определи от употребата на блока |pickrandom|.

.. |pickrandom| image:: ../_images/_imageMicroBit/p49.png

Накрая блокът  |onbutton| би изглеждал така:

.. |onbutton| image:: ../_images/_imageMicroBit/p18.png


.. image:: ../_images/_imageMicroBit/p50.png
      :align: center

За да проверим дължината на страната ``a``, ще завлечем блока |shownumber|.


.. |shownumber| image:: ../_images/_imageMicroBit/15.png

Блокът изглежда така:

.. image:: ../_images/_imageMicroBit/p51.png
      :align: center

За да изчислим периметъра и площта на квадрата, трябва да си припомним, че периметър на квадрат се изчислява като умножим страната му по 4 (4*a), а площта на квадрата е произведение от дължините на страните му  (a*a). Ще използваме умножение за това изчисление. Блокът изглежда така:

.. image:: ../_images/_imageMicroBit/p52.png
      :align: center

За да тестваме програмата, ще използваме симулаторра, натискайки бутона |play|.

.. |play| image:: ../_images/_imageMicroBit/p3.png

.. mchoice:: L5Z2
    :answer_a: Всяка стойност от 0 до 15, без 0.
    :answer_b: Всяка стойност от 0 до 15, вкл. тези стойности.
    :answer_c: Всяка стойност от 0 до 15, без 15.
    :correct: b
    :feedback_a: The answer is not correct!
    :feedback_b: The answer is correct!
    :feedback_c: The answer is not correct!

    Разгледайте блока внимателно:

    .. image:: ../_images/_imageMicroBit/p53.png
          :align: center

    Каква ще бъде стойността на брояча при движение (разтърсване)?
