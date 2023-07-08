# Merge Sort Projesi

## Soru

[16,21,11,8,12,22] -> Merge Sort

1- Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2- Big-O gösterimini yazınız.

## Çözümü

1- Merge Sort: Verinin hafızada sıralı tutulması için geliştirilen sıralama algoritmalarından bir tanesidir. Basitçe sıralanacak olan diziyi ikişer elemanı kalan parçalara inene kadar sürekli olarak ikiye böler daha sonra bu parçaları kendi içlerinde sıralayarak birleştirilir. Sonuçta elde edilen dizi sıralı dizinin kendisidir.

                         [16,21,11,8,12,22] 

1              [16,21,11]                  [8,12,22]

2            [16]    [21,11]                [8]   [12,22]

3            [16]   [21] [11]               [8]   [12]  [22]

4            [16]    [11,21]                [8]    [12,22]

5              [11,21,16]                     [8,12,22]

6                        [8,11,12,16,21,22]

1. 2. ve 3. aşamada elemanlar tek kalana kadar dizin ikiye bölündü. 4. ve 5. aşamada ise elamanlar küçükten büyüğe sıralandı. 6. aşamada ise tüm elemanlar küçükten büyüğe sıralanarak birleşti ve dizin tamamlandı.


2- Elemanlar tek kalana kadar 2'ye bölündüğünden 2^x=n = logn kadar işlem yapılır.
Elamanlar tek kaldıktan sonra birleşerek dizin oluştururken ne kadar n varsa o kadar işlem yapar. Dolayısıyla O(n) diyebiliriz. Bu nedenle dizinin Big-O su **O(nlogn)'dir.**  