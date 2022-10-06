Fundamental-Python-For-Data-Science00 
~hello world~
print ("Hello World")
print ("Hello World")
print(5+1)
print("Ini adalah sebuah baris kode")#ini adalah contoh comment dan tidak akan tercetak
print(10*2+5) #fungsi matematika
print("Academy DQLab") #fungsi mencetak kalimat

~Printing_data_type~
#tipe data Boolean
print(True)
#tipe data String
print("Ayo belajar Python")
print('Belajar Python Sangat Mudah di DQLAB')

#tipe data Integer
print(20)
#tipe data Float
print(3.14)

#tipe data List
print([1,2,3,4,5])
print(["satu", "dua", "tiga"])

#tipe data Tuple
print((1,2,3,4,5))
print(("satu", "dua", "tiga"))

#tipe data Dictionary
print({"nama":"Budi", 'umur':20})

#tipe data Dictionary dimasukan ke dalam variabel biodata
biodata = {"nama":"Andi", 'umur':21} #proses inisialisasi variabel biodata
print(biodata) #proses pencetakan variabel biodata yang berisi tipe data Dictionary
type(biodata) #fungsi untuk mengecek jenis tipe data. akan tampil <class 'dict'>
Klik tombol maka akan keluar hasil seperti ini:

~Melihat_Tipe_Data~
print(type(var_string))
print(type(var_int))
print(type(var_float))
print(type(var_list))
print(type(var_tuple))
print(type(var_dict))

~IF Statement~
i = 10 #inisialisasi variable i yang memiliki nilai 10
if(i==10): #pengecekan nilai i apakah sama dengan 10
    print("ini adalah angka 10") #jika TRUE maka akan mencetak kalimat ini

i = 7 #inisialisasi variable i yang memiliki nilai 10
if(i==10): #pengecekan nilai i apakah sama dengan 10
    print("ini adalah angka 10") #jika TRUE maka akan mencetak kalimat ini

~IF...ELSE...~
i = 10 #inisialisasi variable i yang memiliki nilai 10
if(i==10): #pengecekan nilai i apakah sama dengan 10
    print("ini adalah angka 10") #jika TRUE maka akan mencetak kalimat ini
else:
    print("bukan angka 10") #jika FALSE akan mencetak kalimat ini
i = 5 #inisialisasi variable i yang memiliki nilai 10
if(i==10): #pengecekan nilai i apakah sama dengan 10
    print("ini adalah angka 10") #jika TRUE maka akan mencetak kalimat ini
else:
    print("bukan angka 10") #jika FALSE akan mencetak kalimat ini

~IF...ELIF...ELSE...~
i=5
if(i==5):
     print("ini adalah angka 5")
elif(i>5):
     print("lebih besar dari 5")
else:
     print("lebih kecil dari 5")

i=7
if(i==5):
     print("ini adalah angka 5")
elif(i>5):
     print("lebih besar dari 5")
else:
     print("lebih kecil dari 5")

i=3
if(i==5):
     print("ini adalah angka 5")
elif(i>5):
     print("lebih besar dari 5")
else:
     print("lebih kecil dari 5")


~NESTED IF~
i=2
if(i<7):
	print("nilai i kurang dari 7")
	if (i<3):
		print("nilai i kurang dari 7 dan kurang dari 3")
	else :
		print("nilai i kurang dari 7 tapi lebih dari 3")


~Praktik_Operasi_Matematika~
a=10
b=5
selisih = a-b
jumlah = a+b
kali = a*b
bagi = a/b
print("Hasil penjumlahan a dan b adalah", jumlah)
print("Selisih a dan b adalah :",selisih)
print("Hasil perkalian a dan b adalah :",kali)
print("Hasil pembagian a dan b adalah:",bagi)

~Operasi_Modulus(Sisa Bagi)~
c=10
d=5
modulus=c%d
print("Hasil modulus",modulus)

~Tugas_MID_Praktek~
angka=5
if(angka%2==0):
    print("angka termasuk bilangan genap")
else:
    print("angka termasuk bilangan ganjil")

~While~
#nilai awal j =0
j = 0 
#ketika j kurang dari 6 lakukan perulangan, jika tidak stop perulangan
while j<6: 
    #lakukan perintah ini ketika perulangan
    print("Ini adalah perulangan ke -",j) 
    #setiap kali diakhir perulangan update nilai dengan ditambah 1.
    j=j+1

~for(1)~
for i in range (1,6): #perulangan for sebagai inisialisasi dari angka 1 hingga angka yang lebih kecil daripada 6.

    print("Ini adalah perulangan ke -", i) #perintah jika looping akan tetap berjalan

~for(2) with acces element~
count=[1,2,3,4,5] #elemen list
for number in count: #looping untuk menampilkan semua elemen pada count
    print("Ini adalah element count : ", number) #menampilkan elemen list pada count

~Membuat fungsi Sendiri~
# Membuat Fungsi
def salam():
    print("Hello, Selamat Pagi")
## Pemanggilan Fungsi
salam()

~Parameter pads fungsi~
def luas_segitiga(alas, tinggi): #alas dan tinggi merupakan parameter yang masuk
    luas = (alas * tinggi) / 2
    print("Luas segitiga: %f" % luas);
# Pemanggilan fungsi
##4 dan 6 merupakan parameter yang diinputkan kedalam fungsi luas segitiga
luas_segitiga(4, 6)

~Fungsi dengan Return Value~
#alas dan tinggi merupakan parameter yang masuk
def luas_segitiga(alas, tinggi):
    luas = (alas * tinggi) / 2
    return luas
# Pemanggilan fungsi
##4 dan 6 merupakan parameter yang diinputkan kedalam fungsi luas segitiga 
print("Luas segitiga: %d" % luas_segitiga(4, 6))

~Import_Package_dan_menggunakan_modul~
import math
print("Nilai pi adalah:", math.pi)  # math.pi merupakan sintak untuk memanggil fungsi pi

~Import_dengan_Module_Rename_atau_Alias~
#menggunakan m sebagai module rename atau alias
import math as m
#m.pi merupakan sintak untuk memanggil fungsi
print("Nilai pi adalah:", m.pi)

~Import_Sebagian_Fungsi~
from math import pi
print("Nilai pi adalah", pi)

~Import_Semua_isi_Moduls~
from math import *
print("Nilai e adalah:", e)

~Import CSV~
import requests
from contextlib import closing
import csv
# tentukan lokasi file, nama file, dan inisialisasi csv
url = 'https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv'
# baca file csv secara streaming 
with closing(requests.get(url, stream=True)) as r:
    f = (line.decode('utf-8') for line in r.iter_lines())

    reader = csv.reader(f, delimiter=',')

    # membaca baris per baris
    for row in reader:
        print(row)

~Import_CSV_dari_file~
# tentukan lokasi file, nama file, dan inisialisasi csv
f = open('https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv', 'r')
reader = csv.reader(f)

# membaca baris per baris
for row in reader:
     print (row)

# menutup file csv
f.close()

~Membaca_FIle_csv_dengan_PANDAS
import pandas as pd
pd.set_option("display.max_columns",50)
table = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv")
table.head()
print(table)

~bar_chart~
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
table = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv")
table.head()
x_label = table['NAMA KELURAHAN']
plt.bar(x=np.arange(len(x_label)),height=table['LAKI-LAKI WNI'])
plt.show()

~parameter_dalam_grafik~
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
table = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv")
table.head()
x_label = table['NAMA KELURAHAN']
plt.bar(x=np.arange(len(x_label)),height=table['LAKI-LAKI WNI'])
plt.xticks(np.arange(len(x_label)), table['NAMA KELURAHAN'], rotation=30)
plt.show()

~Menambah_Title_dan_Label_pada_grafik~
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt


table = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/penduduk_gender_head.csv")
table.head()

x_label = table['NAMA KELURAHAN']
plt.bar(x=np.arange(len(x_label)),height=table['LAKI-LAKI WNI'])
plt.xticks(np.arange(len(x_label)), table['NAMA KELURAHAN'], rotation=90)
plt.xlabel('Kelurahan di Jakarta Pusat')
plt.ylabel('Jumlah Penduduk Laki - Laki')
plt.title('Persebaran Jumlah Penduduk Laki- Laki di Jakarta Pusat')

plt.show()

