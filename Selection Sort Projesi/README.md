# Selection Sort Projesi

[22,27,16,2,18,6] -> Insertion Sort

1- a- Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

b- Big-O gösterimini yazınız.

2-Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.

3- [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

## 1. Sorunun Çözümü

a- **Insertion Sort:** Yerleştirerek sıralama işlevi belirli bir anda dizinin belirli bir kısmını sıralı tutarak ve bu kısmı her adımda biraz daha genişleterek çalışmaktadır. Sıralı kısım işlev son bulunca dizinin tamamına ulaşmaktadır. Elemanların sırasına uygun olarak listeye tek tek eklenmesi ile gerçekleştirilen sıralamadır.

[22,*27,16,2,18,6] **ilk adımda** dizinin ilk sırasındaki 22 elemanı sıralanıyor.  

[22,27*,16,2,18,6] **ikinci adımda** 27 elamanını inceliyoruz. 22 ve 27 elamanı sıralı olduğundan dizinde yine bir değişiklik olmadı.

[16,22,27*,2,18,6] **üçüncü adımda** 16 elamanı ile kendinden önceki iki elamanı karşılaştırıyoruz. 16 elemanı 22 ve 27 elamanından küçük olduğundan dizinin ilk sırasına geçiyor.

[2,16,22,27*,18,6] **dördüncü adımda** 2 elamanı ile kendinden önceki üç elamanı karşılaştırıyoruz. 2 elemanı solunda kalan tüm elamanlardan küçük olduğundan dizinin ilk sırasına geçiyor.

[2,16,18,22,27*,6] **beşinci adımda** 18 elamanı ile kendinden önceki dört elamanı karşılaştırıyoruz. 18 elemanı 2 ve 16 elamaından büyük, 22 ve 27 elemanından küçük olduğundan, 16 ve 22 elamanın arasına geçiyor. 

[2,6,16,18,22,27*] **altıncı ve son adımda** 6 elemanı ile kendinden önceki beş elamanı karşılaştırıyoruz. 6 elemanı 2 elemaınından büyük diğer tüm elemanlardan küçük olduğundan dizinin ikinci sırasına geçiyor. Dizindeki tüm elemanlar incelendi ve küçükten büyüğe sıralama oluşturuldu.

b- Yukarıdaki Insertion Sort aşamalarını inlecelersek ilk adımda (n) işlem, ikinci adımda (n-1) işlem, üçüncü adımda (n-2), dördüncü adımda (n-3), beşinci adımda (n-4), son adımda (1) işlem yapıldığını görürüz. Bu işlemlerin ortalaması alacak olursak n.(n+1)/2, özetle bu dizinin **Big-O O(n2)** {n kare 2} olur.

## 2. Sorunun Çözümü

[2,6,16,*18*,22,27] 

18 sayısı dizinin tam ortasında bulunduğundan **average case** kapsamında girer.

## 3. Sorunun Çözümü

Selection Sort: uygulaması oldukça basit olan bu algoritma dizinin ilk elemanının en küçük eleman olduğunu varsayıyor. Ardından tek tek bu elemanı diğer elemanlarla karşılaştırıyor. Eğer karşılaştırdığı eleman daha küçük ise onu en küçük değer olarak alıyor ve ilk eleman yerine artık diğer elemanları onunla karşılaştırıyor. Dizinin sonuna vardığında ise en küçük elemanı dizinin başına yazıyor. Ardından bu işlemi 2. elemandan başlayarak yapıyor ve bulduğu en küçük değeri 2. sıraya koyuyor benzer şekilde işlemi dizinin son elemanına kadar aynı şekilde tekrarlıyor.

[2*,3,5,8,7,9,4,15,6] **ilk adımda** dizinin en küçük elemanı bulunana kadar n işlem yapılır. Bu dizinde en küçük eleman 2 olduğundan, 7 elemanı ile yer değiştirilerek dizinin ilk sırasına yerleştirilir.

[2,3*,5,8,7,9,4,15,6] **ikinci adımda** 2 elemanından sonraki en küçük elaman aranmaya başlanır. 2 elamanından sonra en küçük elaman 3'tür. 3 elemanı kendi yerinde olduğundan işlem yapılmaz.

[2,3,4*,8,7,9,5,15,6] **üçüncü adımda** 3 elemanından sonraki en küçük elaman aranmaya başlanır. 3 elamanından sonra en küçük elaman 4'tür. Dolayısıyla 4 elemanı, 5 elemanı ile yer değiştirerek üçüncü sıraya yerleşir. 

[2,3,4,5*,7,9,8,15,6] **dördüncü adımda** 4 elemanından sonraki en küçük elaman aranmaya başlanır. 4 elamanından sonra en küçük elaman 5'tir. 5 elemanı, 8 elemanı ile yer değiştirerek dördüncü sıraya yerleşir. 



