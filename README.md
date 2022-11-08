# Nama : Tiara Putri
# NIM : 312210064
# Kelas : TI.22.A1

# Tugas4
# **Modul 2**

# **Latihan 1:** 
Membuat program menentukan nilai akhir

     nama = input("Masukkan nama:")
     uts = input("Masukkan nilai UTS:")
     uas = input("Masukkan nilai UAS:")
     tugas = input("Masukkan nilai Tugas:")
  
     akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
     keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
     if akhir > 80:
        huruf = "A"
      elif akhir > 70:
        huruf = "B"
      elif akhir > 50:
        huruf = "C"
      elif akhir > 40:
        huruf = "D"
      else:
        huruf = "E"
    
    print("\nNama :",nama)
    print("Nilai UTS :",uts)
    print("Nilai UAS :",uas)
    print("Nilai Tugas :",tugas)
    print("Nilai Akhir :",akhir)
    print("\nNilai Huruf :",huruf)
    print("Keterangan :",keterangan)

![2022-11-06 (1)](https://user-images.githubusercontent.com/115775237/200157183-218c14c5-d881-4345-9d5f-2eabffe37d10.png)

# **Latihan 2:**

Membuat program menampilkan status gaji karyawan.

    gaji = int(input("Masukkan gaji:"))
    berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
    punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]
    if gaji > 3000000:
        print ("Gaji sudah diatas UMR")
        if berkeluarga:
          print ("Wajib ikutan asuransi dan menabung untuk pensiun")
        else:
          print ("Tidak perlu ikutan asuransi")
        if punya_rumah:
          print ("wajib bayar pajak rumah")
        else:
          print ("tidak wajib bayar pajak rumah")
    else:
      print ("Gaji belum UMR")

![2022-11-06 (2)](https://user-images.githubusercontent.com/115775237/200157215-c4cb0a6b-740f-4450-96b0-82d12d0dbe46.png)

# **Latihan 3:**

penggunaan kondisi OR program membandingkan 3 input bilangan, apabila penjumlahan 2 bilangan hasilnya sama dengan bilangan lainnya, maka cetak pernyataan “BENAR”

     a = int(input("Masukkan bilangan A: "))
     b = int(input("Masukkan bilangan B: "))
     c = int(input("Masukkan bilangan C: "))
     if a+b == c or b+c == a or c+a == b:
          print("BENAR")
     else:
          print("SALAH")
      
![2022-11-06 (3)](https://user-images.githubusercontent.com/115775237/200157242-6198e26f-37a1-4f47-b177-b956056adb22.png)
  
# **Praktikum 2**

Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan
tersebut tampilkan bilangan terbesarnya. Gunakan statement if.

     a, b, c = (
          int(input('Masukkan nilai a: ')),
          int(input('Masukkan nilai b: ')),
          int(input('Masukkan nilai c: '))
     )
     if a > b and a > c:
          print('A yang terbesar')
     elif b > a and b > c:
          print('B yang terbesar')
     else:
          print('C yang terbesar')

![2022-11-08 (2)](https://user-images.githubusercontent.com/115775237/200522792-18622659-df9d-4801-a63c-c0d7533ae534.png)

**Flowchart**

![200482321-1f6c21a7-2288-4347-8d52-f7d50f20dcc1](https://user-images.githubusercontent.com/115775237/200523091-2e92028d-de7d-41c5-a88f-032e74b04ec8.png)

# **Modul3**

# **Latihan 1**

1. Tampilkan n bilangan acak yang lebih kecil dari 0.5.
2. nilai n diisi pada saat runtime
3. anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya
4. gunakan fungsi random() yang dapat diimport terlebih dahulu

     print("bilangan acak yang lebih kecil dari o.5")
     import random

     n = int(input("masukan nilai:"))
     a = 0
     for c in range(n):
          a += 1
          b = random.uniform(.0, .5)
          print("data ke:", a, "==>", b)

     print("selesai")

![2022-11-08 (1)](https://user-images.githubusercontent.com/115775237/200519047-0eaaa049-40c2-4283-8537-708b9a9b0e10.png)

**flowchart**

![200483087-8c454d84-e476-4dd7-96a1-591ed611c4bf](https://user-images.githubusercontent.com/115775237/200520077-f251f0bf-350b-42d3-b67c-ea6f39c8a4ea.png)

# **Latihan 2**

Buat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan. Masukkan angka 0 untuk berhenti.
    
    print("menampilkan bilangan terbesar dari n buah data")
    max=0
    while True:
        a=int(input("masukkan bilangan :"))
        if max < a :
           max = a
        if a==0 :
            break
    print("bilangan terbesar adalah= ", max)

![2022-11-06 (6)](https://user-images.githubusercontent.com/115775237/200157454-130a9ee1-b0bd-446a-a17e-0f7affcace84.png)

**Flowchart**

![200491857-23239d93-dc61-49ed-95f4-534a4469c54c](https://user-images.githubusercontent.com/115775237/200523921-71ce79ed-7509-41d8-b874-9049c754a85c.png)

# **Praktikum 3**

Buat program sederhana dengan perulangan:

Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan modal awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada bulan ketiga baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5, pendapatan meningkat 5%, selanjutnya pada bulan ke 8 mengalami penurunan keuntungan sebesar 2%, sehingga laba menjadi 3%. Hitung total keuntungan selama 8 bulan berjalan usahanya.

    a=1000000000
    for x in range (1,9):
        if(x>=1 and x<=2):
            b=a*0
            print("laba bulan ke-",x, ":", b)
        if(x>=3 and x<=4):
            c=a*0.1
            print("laba bulan ke-",x, ":", c)
        if(x>=5 and x<=7):
            d=a*0.5
            print("laba bulan ke-",x, ":", d)
        if(x==8):
            e=a*0.2
            print("laba bulan ke-",x, ":", e)
    total=b+b+c+c+d+d+d+e
    print("\ntotal :", total)
    
![2022-11-06 (7)](https://user-images.githubusercontent.com/115775237/200157479-2b49efa3-6ae3-43e5-aba8-9c9ccf92048d.png)

**Flowchart**

![200492739-0b575aa2-ee9d-411f-a768-46402ddd5a22](https://user-images.githubusercontent.com/115775237/200523654-91de6485-2606-4443-98d1-f5bbb40673e9.png)

# sekian terima kasih
