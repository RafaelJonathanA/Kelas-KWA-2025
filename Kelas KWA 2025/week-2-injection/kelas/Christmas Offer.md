Order the Christmas special offer of 2014.
https://juice-shop.herokuapp.com/#/score-board?categories=Injection 

Hal-hal yang dilakukan: 
1. Menenemukan query search dari fungsi search yang ada dan didapatkan "127.0.0.1:3000/rest/products/search?q="
2. Query  tersebut dapat kita manfaatkan untuk sql injection  
3. Mengatur payload sehingga dapat menampilkan barang yang sudah dihapus dengan payload 
test')) UNION SELECT * FROM PRODUCTS WHERE deletedAt IS NOT NULL-- 
4. Mendapatkan Id untuk barang yang sudah dihapus dan diketahui barang chrismas special adalah id=10 
5. Melihat bagaimana server menambahkan cart barang dan diketahui menggunakan id barang sehingga bisa kita manfaatkan untuk menambahkan barang yang sudah dihapus namun mengetahui idnya
6. Memanipulasi penambahan cart dengan menggunakan burp suit dan mengganti idnya menjadi 10
7. Kita berhasil menambahkan barang Christmas Special offer of 2014 

Bukti 

![alt text](assets/Chris-1.png)

![alt text](assets/Chris-4.png)

![alt text](assets/Chris-2.png)

![alt text](assets/Chris-3.png)

#### Berhasil 