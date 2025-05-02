# Proje 1: Insertion Sort  
  
## Soru 1  
>[22,27,16,2,18,6]  
> Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.  
  
Insertion Sort aşamaları:  
22<27          -> [22,27,16,2,18,6]  
16<22,27       -> [16,22,27,2,18,6]  
2<16,22,27     -> [2,16,22,27,18,6]  
18<22,27       -> [2,16,18,22,27,6]  
6<16,18,22,27  -> [2,6,16,18,22,27]  
  
## Soru 2
> Dizinin Big-O gösterimini yazınız.  
  
• Best Case: O(n) — Dizinin küçükten büyüğe sıralı geldiği durumdur, her eleman 1 kez kontrol edilir.  
• Average Case: O(n²)  
• Worst Case: O(n²) — Dizinin büyükten küçüğe sıralı geldiği durumdur. Her eleman için dizideki tüm elemanları kontrol etmek gerekir.  
  
Verilen örnekte toplamda 12 kıyaslama yapılmıştır. Bu da worst case olan 5²'den küçüktür.  
  
## Soru 3  
> Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?  
  
[2,6,16,18,22,27]  
  
18 sayısı dizi sıralandıktan sonra dizinin ortasına denk geldiğinden, arama işleminin Time Complexity'si average case kapsamına girer. Eğer sıralı dizide en küçük eleman olan 2 elemanını arıyor olsaydık best case, 27'yi arıyor olsaydık worst case olurdu.  
  
## Soru 4  
>[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.  
  
Selection Sort'a göre ilk 4 Adım:  
  
0.  [7, 3, 5, 8, 2, 9, 4, 15, 6] (seçili eleman 7, min 2, 7>2, yer değiştir)  
1.  [2, 3, 5, 8, 7, 9, 4, 15, 6] (seçili eleman 3, min 4, 3<4 yer değiştirme)  
2.  [2, 3, 5, 8, 7, 9, 4, 15, 6] (seçili eleman 5, min 4, 5>4 yer değiştir)  
3.  [2, 3, 4, 8, 7, 9, 5, 15, 6] (seçili eleman 8, min 5, 8>5 yer değiştir)  
4.  [2, 3, 4, 5, 7, 9, 8, 15, 6] ...  
