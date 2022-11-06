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

