Блокове от категория Basic
==========================

Категорията |Basic| включва блоковете, използвани за стартиране на програми, а също и блоковете, които представят числа, текст или картинки.

Време е да създадем програма, която ще изпише думата „Здравей!“.

За да представим съобщението (на симулатора или на Micro:bit дисплея), трябва да  завлечем блока  |showstring| от категория |Basic| до работния плот и да го вмъкнем в блок |onstart|. Можем да въведем исканото съобщение „Здравей!“ като кликнем на полето за въвеждане на текст.

.. |Basic| image:: ../_images/_imageMicroBit/s2.png
.. |onstart| image:: ../_images/_imageMicroBit/s20.png
.. |showstring| image:: ../_images/_imageMicroBit/p6.png

Ето крайният вид на програмата, показваща съобщението „Здравей!“:

.. image:: ../_images/_imageMicroBit/p5.png
      :align: center

Имаме две възможности да пробваме програмата:

- да я пуснем чрез симулатора, натискайки бутона |play|.

- •	Да я пуснем чрез симулатора, натискайки бутона |download|.

.. |play| image:: ../_images/_imageMicroBit/p3.png
.. |download| image:: ../_images/_imageMicroBit/p4.png
      :width: 200px

Ще използваме симулатора, за да пробваме програмата. Тя се задейства като кликнем на бутона |play|, т.е. се показва съобщението „Здравей!“.

**Задача** Създайте програма, която ще представи съобщението „Здравей!“ безкраен брой пъти. 
**Малко помощ** Блокът |forever| ще повтаря командите, въведени в него, безкраен брой пъти. Работата на този блок никога не спира сама-за да спре да действа, трябва да натиснете бутона stop.

Можеш да сравниш твоите решения с нашите: https://makecode.microbit.org/_9Cw5d6Czda1d


.. |forever| image:: ../_images/_imageMicroBit/s1.png


В категорията |Basic| можете също да намерите и блокове за представяне на изображения |showicons|   или за представяне на изображения, които потребителят може да създаде, включвайки диодите на LED  екрана (|showleds|).


.. |showicons| image:: ../_images/_imageMicroBit/p7.png
.. |showleds| image:: ../_images/_imageMicroBit/s12.png


**Задача** Искате да създадете програма, която представя усмихнато личице на екрана.

Можеш да сравните решението си с нашето:  : https://makecode.microbit.org/_CAdaFfKsY46a


.. mchoice:: L1Z1
    :answer_a: Блок on start.
    :answer_b: Блок forever.
    :feedback_a: The answer is not correct. The onstart block is one of the blocks from the category Basic, and blocks within it are executed only once during the running of the program.
    :feedback_b: Bravo! The forever block is the block within which commands will be executed an infinite number of times. The running of this block will never stop on its own. To stop the running of this block, you need to press the stop button (|stop|).
    :correct: b

    Кой блок, използван за стартиране на програма, ще изберете, ако искате картинките на празен и пълен правоъгълник да се сменят на екрана? 

Отделно от споменатите блокове, в категорията |Basic|, можете да намерите и блокове за представяне на числени стойности |shownumber|, блокове, използвани за забавяне на програмата |pause|, като времевия интервал е представен в милисекунди- 1000 милисекунди са 1 секунда, а също и блока за изчиствени на екрана |clearall|.

.. |shownumber| image:: ../_images/_imageMicroBit/15.png
.. |pause| image:: ../_images/_imageMicroBit/s39.png
.. |clearall| image:: ../_images/_imageMicroBit/s14.png
.. |stop| image:: ../_images/_imageMicroBit/p2.png

**Задача** Изполвайки примера от горния въпрос за сменящите се правоъгълници, опитайте се да забавите времето за смяна с 2 секунди. 
**Малко помощ** Използвайте блока |pause|.

Виж нашето решение тук: https://makecode.microbit.org/_F5h5UKD2Vgau

**Допълнителна задача** Трябва да включите 3/5 LED-а на Micro:bit. Представянето на светещите LED-ове трябва да е уникално!

Сравни решението си с едно от възможните: https://makecode.microbit.org/_29YWXrLHg22U
