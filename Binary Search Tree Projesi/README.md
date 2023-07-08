# Binary Search Tree Projesi

## Soru

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

## Çözümü

Binary Search Tree (BST), her düğümde sol alt ağacın tüm değerlerinin düğüm değerinden küçük, sağ alt ağacın tüm değerlerinin ise düğüm değerinden büyük olduğu bir ağaç yapısıdır.

Soruda verilen dizinde seçilen **root 5'tir.** Her bir eleman 5 ile kıyaslanıp, 5'ten büyükse sağına, küçükse soluna yazılmıştır. 

7>5 olduğundan sağ tarafa,                              
1<5 olduğundan sol tarafa,              
8>5 olduğundan sağ tarafa,
3<5 olduğundan sol tarafa,
6>5 olduğundan sağ tarafa,
0<5 olduğundan sol tarafa,
9>5 olduğundan sağ tarafa,
4<5 olduğundan sol tarafa,
2<5 olduğundan sol tarafa yazılmıştır.

***
           5          
         /   \
        1     7
       / \   / \
      0   3 6   8
         / \     \
        2   4     9

