# hw8
1) использовал рег. выражение \r\n+(\s){1,}, заменил все вхождения на \r\n
![](https://github.com/subna/hw8/blob/master/1.jpg)


2) использовал выражение ([А-Я])([а-я]){1,9}(слав)[а-я]{1,7}, результатов - 594 
![](https://github.com/subna/hw8/blob/master/4.jpg)
численные параметры, кажется, выбраны с запасом, да и не нужны здесь - перестраховка на случай опечаток в документе.
ВАЖНО! выражение не избавляет от нарицательных имен, глаголов, причастий и деепричастий, стоящих в начале предложения; исключение слов, начинающихся с прописной буквы и стоящих в начале путем исключения точки и пробела перед ними, а также просто точки (в документе встречается и такое) - вроде [^\.,\(\.\s)], исключит из выдачи имена собственные, которые тоже могут стоять в начале предложения. Кажется, на языке регулярных выражений (в объеме программы семинара?) решить эту задачу затруднительно, если вообще возможно; количество результатов при этом не столь велико, чтобы нельзя было отсортировать "спорные" случаи вручную.

3) использовал выражение Нов(ѣ|у|е|о|ъ|а)?город, результатов - 85
![](https://github.com/subna/hw8/blob/master/5.jpg)
