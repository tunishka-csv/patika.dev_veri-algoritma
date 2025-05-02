# patika.dev_veri-algoritma
This repository contains projects for Veri Yapıları ve Algoritmalar course in Patika.dev Data Analysis Bootcamp.

## Proje 1: Insertion Sort

# Soru 1
[22,27,16,2,18,6]
Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.

Insertion Sort aşamaları:
22<27          -> [22,27,16,2,18,6]
16<22,27       -> [16,22,27,2,18,6]
2<16,22,27     -> [2,16,22,27,18,6]
18<22,27       -> [2,16,18,22,27,6]
6<16,18,22,27  -> [2,6,16,18,22,27]

# Soru 2
Dizinin Big-O gösterimini yazınız.

• Best Case: O(n) — Dizinin küçükten büyüğe sıralı geldiği durumdur, her eleman 1 kez kontrol edilir.
• Average Case: O(n²)
• Worst Case: O(n²) — Dizinin büyükten küçüğe sıralı geldiği durumdur. Her eleman için dizideki tüm elemanları kontrol etmek gerekir.

Verilen örnekte toplamda 12 kıyaslama yapılmıştır. Bu da worst case olan 5²'den küçüktür.

# Soru 3
Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?

[2,6,16,18,22,27]

18 sayısı dizi sıralandıktan sonra dizinin ortasına denk geldiğinden, arama işleminin Time Complexity'si average case kapsamına girer. Eğer sıralı dizide en küçük eleman olan 2 elemanını arıyor olsaydık best case, 27'yi arıyor olsaydık worst case olurdu.

# Soru 4
[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.
Selection Sort'a göre ilk 4 Adım:
0.  [7, 3, 5, 8, 2, 9, 4, 15, 6] (seçili eleman 7, min 2, 7>2, yer değiştir)
1.  [2, 3, 5, 8, 7, 9, 4, 15, 6] (seçili eleman 3, min 4, 3<4 yer değiştirme)
2.  [2, 3, 5, 8, 7, 9, 4, 15, 6] (seçili eleman 5, min 4, 5>4 yer değiştir)
3.  [2, 3, 4, 8, 7, 9, 5, 15, 6] (seçili eleman 8, min 5, 8>5 yer değiştir)
4.  [2, 3, 4, 5, 7, 9, 8, 15, 6] ...



## Proje 2: Merge Sort

# Soru 1
[16,21,11,8,12,22]
Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

Merge Sort Aşamaları:
```
                        [16,21,11,8,12,22]
                    /                        \
              [16,21,11]                    [8,12,22]
            /           \                  /         \  
       [16,21]         [11]             [8,12]       [22]
      /      \          |              /      \       |
   [16]      [21]      [11]          [8]     [12]    [22]
-----------------------------Merge sub-series------------------------------------
            [11,16,21]                     [8,12,22]      
---(8<11 -> 8 en sola, 11<12 -> 11 ikinci, 12<16 -> 12 üçüncü, 16>22 -> 16 dördüncü, 21>22 -> 21 beşinci ve 22 altıncı eleman)---
                        [8,11,12,16,21,22]
```

# Soru 2
Dizinin Big-O gösterimini yazınız.

O(nlogn)


## Proje 3: Binary Search Tree

# Soru 1
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

Dizideki ilk eleman 7 root olarak seçilir.
Dizideki ikinci eleman 5, 5<7 olduğundan root'un sağına yazılır. 
Üçüncü eleman 1, 1<5,7 olduğundan 5'in soluna yazılır. 
Dördüncü eleman 8, 7<8 olduğundan rootu'un sağına yazılır.
Beşinci eleman 3, 1<3<7,5 olduğundan, 1'in sağına yazılır.
Altıncı eleman 6, 5<6<7 olduğundan, 5'in sağına yazılır.
Yedinci eleman 0, 0<1,5,7 olduğundan, 1'in soluna yazılır.
Sekizinci eleman 9>7,8 olduğundan 8'in sağına yazılır.
Dokuzuncu eleman 4, 3<4<5,6,7 olduğundan 3'ün sağına yazılır.
Onuncu eleman 2, 2<3,4,5,6,7 olduğundan 3'ün soluna yazılır.

```
        7
       / \
      5   8
     / \    \
    1   6    9
   / \
  0   3
     / \
    2   4
```
