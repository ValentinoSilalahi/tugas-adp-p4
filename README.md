print ( "Nama : Valentino Silalahi" )
print ( "Nim  : 2310431015" )
print ( "Program Bus PT.ANS Lintas Sumatera" )

print("\nTujuan Bus PT.ANS : ")
print("1. Medan   (Rp300.000) ")
print("2. Padang  (Rp50.000 ) ")
print("3. Jambi   (Rp250.000) ")
print("4. Sibolga (Rp100.000) ")
print("5. Pakkat  (Rp200.000) ")
print("6. Solok   (Rp70.000 ) ")

tujuan = input( "Masukkan tujuan anda : " )
if tujuan == "Medan":
    htujuan = 300000
elif tujuan == "Padang":
    htujuan = 50000
elif tujuan == "Jambi":
    htujuan = 250000
elif tujuan == "Sibolga":
    htujuan = 100000
elif tujuan == "Pakkat":
    htujuan = 200000
elif tujuan == "Solok":
    htujuan = 70000
else:
    print("Tujuan anda tidak terdaftar")

print("Tujuan anda adalah = ", tujuan, " || Dengan harga = Rp", htujuan)

print("\n-----------------------------------\n")

print("Kelas Bus PT.ANS :")
print("1. Ekonomi (Rp10.000) ")
print("2. Bisnis  (Rp20.000) ")
print("3. First   (Rp30.000) ")

kelas = input("Masukkan kelas anda: ")

if kelas == "Ekonomi":
    hkelas = 10000
elif kelas == "Bisnis":
    hkelas = 20000
elif kelas == "First":
    hkelas = 30000
else:
    print("Kelas anda tidak terdaftar")

print("Kelas anda adalah = ", kelas, " || Dengan harga = Rp", hkelas)

tiket = int(input("Jumlah tiket anda = "))

print("\n-----------------------------------\n")

total = (htujuan + hkelas) * tiket

if tiket > 5:
    diskon = 0.10 * total
elif tiket >= 3:
    diskon = 0.05 * total
else:
    diskon = 0 * total

total_akhir = total - diskon

print("Tujuan :", tujuan)
print("Kelas :", kelas)
print("Jumlah tiket :", tiket)
print("Total harga tiket anda = Rp", total)
print("Diskon yang didapat = Rp", diskon)
print("Total harga setelah diskon = Rp", total_akhir)
