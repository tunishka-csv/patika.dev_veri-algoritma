# Proje 3: Binary Search Tree

## Soru 1
> [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
> Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

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
