# Proje 2: Merge Sort

## Soru 1
[16,21,11,8,12,22]
> Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

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

## Soru 2
> Dizinin Big-O gösterimini yazınız.

O(nlogn)
