
```js no-beautify
"" + 1 + 0 = "10" // (1)
"" - 1 + 0 = -1 // (2)
true + false = 1
6 / "3" = 2
"2" * "3" = 6
4 + 5 + "px" = "9px"
"$" + 4 + 5 = "$45"
"4" - 2 = 2
"4px" - 2 = NaN
7 / 0 = Infinity
" -9  " + 5 = " -9  5" // (3)
" -9  " - 5 = -14 // (4)
null + 1 = 1 // (5)
undefined + 1 = NaN // (6)
```

1. ""değer taşımadığı halde string yapıdadır. Toplama işlemi burada birleştirme şeklinde gerçekleşir."" değer taşımadığı için  `"" + 1 = "1"` olacaktır.  Aynı şekilde "1" + 0 = "10"
2. Çıkarma işlemi çoğu matamatik işleminde olduğu gibi string değerleri sayıya dönüştürür. "" bu durumda `0` olarak işleme girer. 0-1+0 =-1
3. sayısal bir eleman string bir değerle toplama işlemine girdiğinde stringe dönüşür ve birleştirme işlemi gerçekleşir.(string değerdeki boşlukların korunduğuna dikkat edin.)
4. " -9 " Çıkarma işlemine girdiğinde sayısal olan `-9` değerini alır -9 -5 = -14
5. `null` un numaraya donuşumunün karşılığı `0` dır 0+1=1
6. `undefined` in numaraya donuşumunün karşılığı `NaN` dır. `NaN`+1 = `NaN`
