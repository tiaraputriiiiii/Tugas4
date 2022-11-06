# Tugas4
**Modul 2**

**Latihan 1: Membuat program menentukan nilai akhir**

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

**Latihan 2: Membuat program menampilkan status gaji karyawan.**

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

**Latihan 3: penggunaan kondisi OR program membandingkan 3 input bilangan, apabila penjumlahan 2 bilangan hasilnya sama dengan bilangan lainnya, maka cetak pernyataan “BENAR”**

    a = int(input("Masukkan bilangan A: "))
    b = int(input("Masukkan bilangan B: "))
    c = int(input("Masukkan bilangan C: "))
    if a+b == c or b+c == a or c+a == b:
      print("BENAR")
    else:
      print("SALAH")
  
**Praktikum 2**
Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan
tersebut tampilkan bilangan terbesarnya. Gunakan statement if. 

    data =[]
    for i in range (3):
        x=int(input("masukkan bilangan :"))
        data.append(x)
    print ("data sebelum diurutkan :", data)
    list.sort(data)
    print ("data setelah diurutkan :", data)

**Modul3**
**Latihan 1: latihan1.py**
1. Tampilkan n bilangan acak yang lebih kecil dari 0.5.
2. nilai n diisi pada saat runtime
3. anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya
4. gunakan fungsi random() yang dapat diimport terlebih dahulu

    import random
    jumlah = int (input("Masukkan jumlah n:"))
    for i in range(5):
        i=random.uniform(0.0,0.5)
    print("Data Ke: 1=>", i)
    jawab="betul"
    hitung = 0
    while (jawab):
        hitung +=1
    jawab =input("Selesai")
    
**Latihan 2: latihan2.py**
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

**Praktikum 3**

**Buat program sederhana dengan perulangan: program1.py**
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
    
