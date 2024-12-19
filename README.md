# siRNA
Подбор микро-РНК для РНК-интерференции

ВВЕДЕНИЕ

РНК-интерференция - важный механизм регуляции экспрессии генов. В частности он осуществляется за счет малых интерферирующих РНК (миРНК, англ. siRNA) – двуцепочечных молекул РНК длиной 20–25 пар оснований, роль которых предположительно связана с защитой клетки и поддержанием целостности генома за счет подавления экзогенных нуклеиновых кислот и нежелательных транскриптов. миРНК являются агентами специфического сайленсинга комплементарной матричной РНК. При взаимодействии миРНК и мРНК происходит деградация матричной РНК, прекращается трансляция закодированного ею белка на рибосоме (Laganà A. et al, 2015). РНК-интерференция является важной частью механизмов противовирусной защиты. 
На сегодняшний день возможно создание экзогенных миРНК, что позволяет использовать их для антивирусной терапии. Существует несколько способов получения миРНК, таких как химический синтез, транскрипция in vitro, экспрессионные векторы миРНК и кассеты экспрессии ПЦР. Независимо от того, какой метод используется, первым шагом в разработке миРНК является выбор сайта-мишени миРНК (Mehta A. et al, 2021).  Для этого в последовательности от старт-кодона осуществляется поиск двух последовательно стоящих аденинов, так как динуклеотид и 19 прилегающих дальше по цепи нуклеотидов - потенциальный сайт-мишень миРНК. В результате исследований научного центра Ambion выяснено, что миРНК с 30-50% содержанием гуанинов и цитозинов более активны, чем с более высоким высоким GC-составом, следовательно, при выборе сайта-мишени предпочтение отдается первым. Также важным этапом разработки миРНК является контроль: выбранная миРНК не должна быть комплементарна другим последовательностям в транскриптоме. Финальный этап - конструирование шпилек в молекуле миРНК. Большинство созданных исследователями конструкций имели два инвертированных повтора, разделенных короткой спейсерной последовательностью, и заканчивались цепочкой политимидина , которая служила сайтом терминации транскрипции. Эти конструкции производят РНК-транскрипты, которые должны сворачиваться в короткую шпильку миРНК, как показано на рисунке 1. 

DNA sequence of target site
"""
            ____________  
            |   19 nt  |
5'--------AA-------------3'
3'--------TT-------------5'

RNA target
5'--------AA-------------3'

Hairpin siRNA

      5'------------- U U C A 
        |||||||||||||        A
3'UUUUU'------------- A G A G  """
 
Рис. 1. Схема типичной шпилечной миРНК⁴

Задачи:

-Поиск потенциальных сайтов-мишеней миРНК.
-Проверка выбранных последовательностей на содержание гуанин-цитозиновых связей и выбор подходящих.
-Выравнивание подходящих последовательности на транскриптом человека для предотвращения комплиментарности.
-Конструирование миРНК шпилек.
-Разработка интерфейса

МАТЕРИАЛЫ И МЕТОДЫ

Данная работа посвящена разработке программы для подбора сайта-мишени миРНК. Код написан на языке Python 3.11.4, интерфейс приложения разработан на основе графической библиотеки Tkinter. Программа состоит из двух смысловых частей: первая - это поиск подходящего участка по таким параметрам, как  наличие аденинового динуклеотида и количество гуанин-цитозиновых связей, дальнейшее формирование шпильки; вторая - локальное выравнивание подобранной шпильки на транскриптом человека. 

РЕЗУЛЬТАТЫ И ОБСУЖДЕНИЕ

Разработана программа, осуществляющая выбор подходящего сайта-мишени миРНК, формирует шпильку миРНК 

ЛИТЕРАТУРА

1. Elbashir, et al. (2001) Functional anatomy of siRNA for mediating efficient RNAi in Drosophila melanogaster embryo lysate. EMBO J 20: 6877-6888.

2. Laganà A. et al. Computational design of artificial RNA molecules for gene regulation //RNA Bioinformatics. – 2015. – С. 393-412.

3. Mehta A., Michler T., Merkel O. M. siRNA Therapeutics against Respiratory Viral Infections—What Have We Learned for Potential COVID‐19 Therapies? //Advanced healthcare materials. – 2021. – Т. 10. – №. 7. – С. 2001650.

4. Using siRNA for gene silencing is a rapidly evolving tool inx` molecular biology⁴




