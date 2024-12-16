# mergeshort
Kodluyoruz Eğitimi kapsamında mergeshort ödevi 
# Merge Sort Aşamaları: Verilen dizi: [16, 21, 11, 8, 12, 22]

Merge Sort, böl ve yönet (Divide and Conquer) prensibine dayanır. Diziyi sürekli olarak ikiye böler ve her iki parçayı sıraladıktan sonra bunları birleştirerek sıralı hale getirir.

Adım 1: Bölme Aşaması İlk olarak diziyi ikiye bölelim:

Sol parça: [16, 21, 11] Sağ parça: [8, 12, 22] Adım 2: Sol Parçayı Bölme [16, 21, 11] dizisini ikiye bölelim:

Sol parça: [16] Sağ parça: [21, 11] [16] zaten tek elemanlı olduğu için sıralıdır.

Adım 3: Sağ Parçayı Bölme (Sol Parçanın Devamı) [21, 11] dizisini ikiye bölelim:

Sol parça: [21] Sağ parça: [11] Her iki parça da tek elemanlı olduğu için sıralıdır.

Adım 4: Birleştirme (Sol Parçanın Birleştirilmesi) Şimdi, [21] ve [11] parçalarını birleştirelim:

11, 21'den küçük olduğu için 11 ilk sıraya yerleşir, ardından 21 gelir. Birleşmiş dizi: [11, 21] Adım 5: Birleştirme (Sol Parçanın Tamamlanması) Şimdi [16] ve [11, 21] dizilerini birleştirelim:

11, 16'dan küçük olduğu için 11 ilk sıraya gelir. 16, 21'den küçük olduğu için 16 ikinci sıraya yerleşir. Son olarak 21 gelir. Birleşmiş dizi: [11, 16, 21] Adım 6: Sağ Parçayı Bölme Şimdi, sağdaki [8, 12, 22] dizisini ikiye bölelim:

Sol parça: [8] Sağ parça: [12, 22] [8] zaten tek elemanlı olduğu için sıralıdır.

Adım 7: Sağ Parçayı Bölme (Sağ Parçanın Devamı) [12, 22] dizisini ikiye bölelim:

Sol parça: [12] Sağ parça: [22] Her iki parça da tek elemanlı olduğu için sıralıdır.

Adım 8: Birleştirme (Sağ Parçanın Birleştirilmesi) Şimdi [12] ve [22] dizilerini birleştirelim:

12, 22'den küçük olduğu için 12 önce gelir. Ardından 22 gelir. Birleşmiş dizi: [12, 22] Adım 9: Birleştirme (Sağ Parçanın Tamamlanması) Şimdi [8] ve [12, 22] dizilerini birleştirelim:

8, 12'den küçük olduğu için 8 önce gelir. Ardından 12 gelir, ve sonra 22 gelir. Birleşmiş dizi: [8, 12, 22] Adım 10: Son Birleştirme Son olarak, [11, 16, 21] ve [8, 12, 22] dizilerini birleştirelim:

8, 11'den küçük olduğu için 8 önce gelir. 11, 12'den küçük olduğu için 11 önce gelir. 12, 16'dan küçük olduğu için 12 önce gelir. 16, 21'den küçük olduğu için 16 önce gelir. 21, 22'den küçük olduğu için 21 önce gelir. Son olarak 22 gelir. Sonuçta sıralı dizi: [8, 11, 12, 16, 21, 22]

# Big-O Gösterimi: 
Merge Sort'un zaman karmaşıklığı her zaman O(n log n)'dir. Çünkü her adımda diziyi ikiye böleriz (log n) ve her iki parça üzerinde işlem yaparız (n). Bu nedenle toplam karmaşıklık O(n log n) olur.

# Best Case (O(n log n)): 
Merge Sort her durumda aynı şekilde çalıştığı için, dizinin sıralı olup olmaması fark etmez. Worst Case (O(n log n)): Aynı şekilde, dizinin sıralı ya da sırasız olması fark etmez, karmaşıklık her durumda O(n log n) olur. Average Case (O(n log n)): Ortalama durumda da karmaşıklık yine O(n log n)'dir. Sonuç olarak, Merge Sort'un tüm durumlarda zaman karmaşıklığı O(n log n)'dir.
