# Merge-Sort
Merge Sort laogritma
Öncelikle, Merge Sort algoritması divide and conquer yaklaşımını kullanır ve genelde aşağıdaki adımları izler:

Dizi, tek elemanlı (ve dolayısıyla sıralanmış) alt kümeler oluşana kadar bölünür.
Bu alt kümeler, sıralanmış daha büyük kümeler oluşturmak için birleştirilir.
Bu işlem, tüm dizi sıralanana kadar devam eder.
Verilen diziyi Merge Sort ile sıralama aşamalarını aşağıdaki gibi adımlarla gösterebiliriz:

Verilen dizi: [16,21,11,8,12,22]

Adım - Bölme:
[16, 21, 11, 8, 12, 22] -> [16, 21, 11], [8, 12, 22]

Adım - Bölme:
[16, 21, 11] -> [16], [21, 11]
[8, 12, 22] -> [8], [12, 22]

Adım - Bölme:
[21, 11] -> [21], [11]
[12, 22] -> [12], [22]

Şimdi elimizde sadece tek elemanlı listeler var. Bunları sıralı şekilde birleştirmeye başlayabiliriz.

Adım - Birleştirme:
[16], [21, 11] -> [16], [11, 21]
[8], [12, 22] -> [8], [12, 22]

Adım - Birleştirme:
[16, 21, 11] -> [11, 16, 21]
[8, 12, 22] -> [8, 12, 22]

Adım - Birleştirme:
[11, 16, 21], [8, 12, 22] -> [8, 11, 12, 16, 21, 22]

Sonuç olarak, sıralanmış dizi: [8, 11, 12, 16, 21, 22]

Merge sort algoritmasının Big-O gösterimi genellikle O(n log n)'dir. Bu, diziyi bölme ve birleştirme işlemlerinin ikisinin de en kötü durumda n log n zaman alacağını gösterir.
