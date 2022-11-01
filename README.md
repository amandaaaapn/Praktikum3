
# Cara Installasi Pycharm
Anda harus install Pycharm di https://www.jetbrains.com/pycharm/download/#section=windows  , Dan anda pilih yang Community

![Screenshot (43)1](https://user-images.githubusercontent.com/115678845/199135643-06e741d8-c06e-48de-9abe-0bf0fdba6c85.png)

next saja semua perintahnya 

![Screenshot (44)1](https://user-images.githubusercontent.com/115678845/199135830-dffa231e-9b0a-4830-9379-e13d2c98ecf2.png)

tunggu hingga selesai

![Screenshot (45)1](https://user-images.githubusercontent.com/115678845/199136044-cc2243da-8475-4a5a-8e72-ae03038706db.png)

Jika sudah selesai maka program siap di gunakan

# Cara Menjalankan Pycharm 
# Latihan 1

Pertama-tama anda harus Klik New project lalu kasih nama project anda(sesuai yang anda mau), Dan anda harus pilih yang Previously Configurred interperter lalu klik yang add interperter dan pilih yang System interperter dan anda klik yang versi Python anda seperti gambar di bawah ini

![Screenshot (47)](https://user-images.githubusercontent.com/115678845/199136231-9014bf49-0815-40cb-a52b-81f811f2ed46.png)

![Screenshot (54)1](https://user-images.githubusercontent.com/115678845/199136603-b0118646-c15e-4a90-a18a-1532bad7d600.png)

Selanjutnya anda membuat file Python baru di project anda tadi dan anda kasih nama file sesuai yang anda inginkan

![Screenshot (49)1](https://user-images.githubusercontent.com/115678845/199137102-654eb99a-1199-4689-bab4-04eeaa964d2c.png)

masukan code dari latihan1 anda lalu Run

	# penggunaan end

	print('A', end='')
	print('B', end='')
	print('C', end='')
	print()
	print('X')
	print('Y')
	print('Z')

	# penggunaan separator
	w, x, y, z = 10, 15, 20, 25
	print(w, x, y, z)
	print(w, x, y, z, sep=',')
	print(w, x, y, z, sep='')
	print(w, x, y, z, sep=':')
	print(w, x, y, z, sep='-----')

	# string format
	print(0, 10 ** 0)
	print(1, 10 ** 1)
	print(2, 10 ** 2)
	print(3, 10 ** 3)
	print(4, 10 ** 4)
	print(5, 10 ** 5)
	print(6, 10 ** 6)
	print(7, 10 ** 7)
	print(8, 10 ** 8)
	print(9, 10 ** 9)
	print(10, 10 ** 10)

	# string format
	print('{0:>3} {1:>16}'.format(0, 10 ** 0))
	print('{0:>3} {1:>16}'.format(1, 10 ** 1))
	print('{0:>3} {1:>16}'.format(2, 10 ** 2))
	print('{0:>3} {1:>16}'.format(3, 10 ** 3))
	print('{0:>3} {1:>16}'.format(4, 10 ** 4))
	print('{0:>3} {1:>16}'.format(5, 10 ** 5))
	print('{0:>3} {1:>16}'.format(6, 10 ** 6))
	print('{0:>3} {1:>16}'.format(7, 10 ** 7))
	print('{0:>3} {1:>16}'.format(8, 10 ** 8))
	print('{0:>3} {1:>16}'.format(9, 10 ** 9))
	print('{0:>3} {1:>16}'.format(10, 10 ** 10))
  
  ![Screenshot (55)](https://user-images.githubusercontent.com/115678845/199137319-10226865-f545-4fb7-8023-c645b2211dc6.png)
![Screenshot (56)](https://user-images.githubusercontent.com/115678845/199137326-b044fafb-a36e-4116-a948-9dd357bf18ca.png)

lalu hasil run nya

![Screenshot (57)](https://user-images.githubusercontent.com/115678845/199137433-3ca643e8-b7a2-432e-9817-6578f9550686.png)

# Latihan 2 
buat latihan baru "latihan2"

lalu masukkan code program

	a=input("masukkan nilai a:")
	b=input("masukkan nilai b:")
	print("variabel a=",a)
	print("variabel b=",b)
	print("hasil penggabungan {1}&{0}=%s".format(a,b) %(a+b))

	#konversi nilai variabel
	a=int(a)
	b=int(b)
	print("hasil penjumlahan {1}+{0}=%s".format(a,b) %(a+b))
	print("hasil penjumlahan {1}/{0}=%s".format(a,b) %(a/b))

![Screenshot (58)](https://user-images.githubusercontent.com/115678845/199137715-d3820552-eb16-4348-be51-6a008e13e814.png)

lalu hasil run nya menjadi

![Screenshot (59)](https://user-images.githubusercontent.com/115678845/199137734-30af4c9b-8df0-4069-b61e-31273472eeaf.png)

# Latihan 3
buat file baru "latihan3"

masukkan code programnya

	string = ""

	x = int(input("Masukkan angka :"))
	bar = x
	# Looping Baris
	while bar >= 0:
	# Looping Kolom Spasi Kosong
	kol = bar
	while kol > 0:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri
	kiri = 1
	while kiri < (x - (bar-1)):
		string = string + " * "
		kiri = kiri + 1
	# Looping Kolom Bintang Sisi Kanan
	kanan = 1
	while kanan < kiri -1:
		string = string + " * "
		kanan = kanan + 1

	string = string + "\n\n"
	bar = bar - 1

	bar = 1
	# Looping Baris
	while bar <= x:
	kol = bar+1
	# Looping Kolom Spasi Kosong
	while kol > 1:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri
	kiri = 0
	while kiri < (x - bar):
		string = string + " * "
		kiri = kiri + 1
	# Looping Kolom Bintang Sisi Kanan
	kanan = kiri
	while kanan > 1:
		string = string + " * "
		kanan = kanan - 1

	string = string + "\n\n"
	bar = bar + 1
	print (string)
  
![Screenshot (60)](https://user-images.githubusercontent.com/115678845/199138205-987278b9-ef58-43d7-9e56-4311f8472d1f.png)

![Screenshot (61)](https://user-images.githubusercontent.com/115678845/199138208-9e23aae6-6f66-4261-857f-a52fe9a73a31.png)

*Hasil Run*

![Screenshot (62)](https://user-images.githubusercontent.com/115678845/199138206-29c6bc2f-1651-402b-8cc1-c73c68a8a0f5.png)

![Screenshot (63)](https://user-images.githubusercontent.com/115678845/199138207-ae65a0d8-67b9-4e15-8c2a-fd77b679ec56.png)

# Menghitung Luas Dan Keliling Lingkaran
buat file baru "praktikum3"

	print('menghitung luas dan keliling lingkarang')
	print('________________________________________')

	r=float(input('masukkan nilai jari - jari :'))

	phi=3.14
	diameter=2*r

	print('\nluasnya =', str("%.2f" % luas))
	print('kelilingnya =', str("%.2f" % keliling))

![Screenshot (64)](https://user-images.githubusercontent.com/115678845/199138688-93126249-7019-44f0-bf80-23d0887d900d.png)

*Hasil Run*

![Screenshot (65)](https://user-images.githubusercontent.com/115678845/199138742-bc3d961d-28b2-4e01-a154-d0ea8728febb.png)

# Flowchart Menghitung luas dan keliling lingkaran

![199132888-b964fb68-df4c-4b40-a824-8365a2337d9c](https://user-images.githubusercontent.com/115678845/199138956-0b4f8353-690b-4525-8c82-b10a7c26f92d.png)

### Terima Kasih
