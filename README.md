# Pythons-Conditioning-Looping  
 
Kali ini kita akan membedah sebuah code yang akan menghitung total pemasukkan dan pengeluaran  dari sebuah list yang berisi angka positf sebagai pemasukkan dan angka negatif sebagai pengeluaran.

Jadi kita perlu menentukan langkah-langkah terlebih dahulu
1. Membuat variabel yang menampung angka positif (pemasukan) dan negatif (pengeluaran) dalam bentuk list 
    
       list_cash_flow = [ 2500000, 5000000, -1000000, -2500000, 5000000, 10000000, -5000000, 7500000, 10000000, -1500000, 25000000, -2500000 ] 

   kalian tidak harus terpaku pada default list, kalian bisa mengisinya dengan angka-angka yang sesuai dengan keinginan

2. Lalu variabel yang akan menampung total pengeluaran dan total pemasukkan yang berisi angka 0 

       total_pengeluaran, total_pemasukkan = 0, 0

   kalian juga bisa membuat dua variabel secara terpisah seperti biasa, namun pada kali ini kita mencoba sedikit perbedaan denggan menggabungkan 2 variabel dalam satu baris. Sebenarnya hal ini tidak menjadi masalah terserah yang mana yang akan digunakan

       total_pengeluaran = 0
       total_pemasukkan = 0 
   di isi dengan angka nol karna nanti kita akan menambahkannya dengan data yang ada dalam variabel list_cash_flow tadi
 
3. Selanjutnya kita perlu membuat perulangan dan pengkondisian atau menggunakan if, yang secara otomatis akan memasukkan angka negatif ke variabel total_pengeluaran dan angka positif ke variabel total_pemasukkan.
 
       for dana in list_cash_flow:
         if dana > 0:
             total_pemasukan += dana
         else:
             total_pengeluaran += dana

   penjelasan: pada perulangan / loop menggunakan for kita seolah membuat sebuah variabel baru, pada kali ini yaitu dana. Jadi setiap angka / dana yang ada dalam variabel list_cash_flow, jika besar dari 0 maka variabel total_pemasukkan akan ditambahkan dengan berapa jumlah angka positif dari variabel list_cash_flow
   selanjutnya statement else, jika dana kecil dari 0 (dimana yang dimaksud disini adalah angka negatif, tentu kecil dari 0), maka variabel total_pengeluran akan ditambahkan dengan berapa jumlah angka negatif dari variabel list_cash_flow
   

4. lalu kita akan membuat variabel total_pengeluaran yang sebelumnya berisi angka negatif diubah menjadi angka positif, agar kita dapat membandingkannya dengan total_pemasukkan

          total_pengeluaran *= -1

   variabel total_pengeluaran tadi yang sudah kita looping berisi angka negatif, caranya agar dapat dirubah menjadi angka positif adalah dengan mengkalikannya dengan angka negaif.
   jadi negatif * negatif = positif
   menggunakan -1 agar tidak merubah angka yang sudah ada pada variabel total_pengeluaran. Kita hanya butuh angka yang positif tanpa merubah angka yang ada didalamnya, maka digunakanlah angka -1.
   contohnya total_pengeluaran = -100
   -100 * -1 = 100

5. kemudian kita panggil / print variabel total_pengeluran dan total_pemasukkan

          print(total_pengeluran)
          print(total_pendapatan)
   sebenarnya pada langkah 3 kita sudah bisa mendapatkan hasilnya, tapi dengan menggunakan langkah 4 maka hasilnya akan lebih baik dan mudah dipahami.
   kalian bisa mencoba untuk menghapus code di langkah 4 dan lihat hasilnya
   
   sumber code : https://academy.dqlab.id/main/livecode/157/294/1311?pr=0

Hasil buatan sendiri

![image](https://user-images.githubusercontent.com/81607253/133889728-051820e9-1e72-4d4a-a397-7269a0e8b44f.png)
