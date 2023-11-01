TUGAS STRUKTUR KONDISI
Latihan 1 
Buat program sederhana dengan input 2 buah bilangan, kemudian tentukan bilangan terbesar dari kedua bilangan tersebut menggunakan statement if.

#Masukan input 
bil1 = int (input("Masukan bilangan : "))
bil2 = int (input("Masukan bilangan : "))

#Nilai terbesar

if (bil1 > bil2):
   print("Bilangan terbesar :",bil1)

#Nilai terkecil

if (bil1 < bil2):
   print("Bilangan terbesar :",bil2)
   ![Screenshot (76)](https://github.com/RadityaTansyLizara/latihan7/assets/147571863/6138c92b-f82b-4624-b6e3-d91dde6ed185)

Latihan2
Buat program untuk mengurutkan data berdasarkan input sejumlah data (minimal 3 variable input atau lebih), kemudian tampilkan hasilnya secara berurutan mulai dari data terkecil.

#Masukan inputan
bil1 = int(input("Bilangan ke-1: "))
bil2 = int(input("Bilangan ke-2: "))
bil3 = int(input("Bilangan ke-3: "))

#Buat variable data
data = [bil1, bil2, bil3]

#Menampilkan data
print("Data sebelum di urutkan :", data)
list.sort(data)
print("Data setelah di urutkan :", data)
list.sort Syntax ini berfungsi untuk mengurutkan data
![Screenshot (77)](https://github.com/RadityaTansyLizara/latihan7/assets/147571863/244ec842-bfa7-4d22-a878-fa288efa661d)

TUGAS PERULANGAN
Latihan1
Buat program dengan perulangan bertingkat (nested) for yang menghasilkan output sebagai berikut:

baris = 10
kolom = baris

for bar in range(baris):
    for col in range(kolom):
        tab = bar+col
        print("{0:>5}".format(tab), end='')
    print()
Penjelasan

Pendeklarasian variable
baris = 10
kolom = baris
Untuk perulangan baris dan kolom menggunakan for
for bar in range(baris):
    for col in range(kolom):
        tab = bar+col        
Untuk menampikan hasil dari perulangan
Agar terlihat rapih menggunakan format string rata ke kanan sebanyak 5 karakter
Agar tidak membuat baris baru menggunakan end='' (baris)
  print("{0:>5}".format(tab), end='')
print()    
![Screenshot (78)](https://github.com/RadityaTansyLizara/latihan7/assets/147571863/cf11ae30-b477-4f24-8a2f-454d3a32c204)

Latihan2
Tampilkan n bilangan acak yang lebih kecil dari 0.5. nilai n diisi pada saat runtime anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya.

import random
print("===========================================")
print("= Bilangan acak yang lebih kecil dari 0,5 =")
print("===========================================")

jum = int( input("Masukan nilai: "))
i = 0
while i in range(jum):
    i += 1
    angkarandom = random.uniform(0,0.5)
    print("Bilangan ke :", i, " : ", angkarandom)
    ![Screenshot (80)](https://github.com/RadityaTansyLizara/latihan7/assets/147571863/1d3fe0b1-2309-42d0-9e2a-bde86d8b3de1)
    import random Untuk membuat bilangan acak
jum = int(input("Masukan nilai: ")) Menentukan jumlah input & di konversikan dalam bilangan bulat-dimasukan ke variable jum/jumlah
while i in range(jum) Pengulangan
Menampilkan urutan sesuai inputan dengan hasil di bawah 0.5
angkarandom = random.uniform(0,0.5)
    print("Bilangan ke :", i, " : ", angkarandom)



