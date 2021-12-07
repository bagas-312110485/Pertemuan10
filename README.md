# Pertemuan10 (Latihan 1)

pada latiahan 1 saya diberi soal sebagai berikut: 

![Gambar 1](gambar/Latihan1.png)

saya membuat data kontak awal
````py
    b={'ari':'085267888','dina':'087677776'}
````

saya diberi soal untuk menampilkan kontak ari
````py
    print(b['ari'])
````

saya disuruh menambah kontak atas nama riko
````py
    b['riko']='087654544'
````

ubah kontak dina
````py
    b['dina']='088999776'
````

tampilkan semua nama
````py
    print(b.keys())
````

tampilkan semua nomor
````py
    print(b.values())
````

nenampilkan semua nama dan nomor
````py
    print(b)
````

menghapus kontak dina
````py
    del b['dina']
````

## Tampilan Visual code 

![Gambar 2](gambar/TampilanLatihan1.png)

## Output

![Gambar 3](gambar/OutputLatihan1.png)

# Tugas Praktikum 

Pada tugas praktium saya diberi soal sebagai berikut:

![Gambar 4](gambar/TugasPraktikum.png)

## Flowchart 

![Gambar 5](gambar/flowchart.png)

### Penjelasan 

pertama saya membuat looping agar program terus berjalan:
````py
    while True:
    c = input("\n(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")                                
````

lalu saya membuat format if untuk memasukan pilihan , sebagai contoh apabila memilih (t) akan menambah data
````py
    if (c.lower() == 't'):                                               
        print('\nTambah Data Mahasiswa Baru')
        nama= input("Masukkan Nama\t\t: ")                                        
        nim= input("Masukkan NIM\t\t: ")                                         
        nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))                              
        nilaiUts= int(input("Masukkan Nilai UTS\t: "))                                   
        nilaiUas= int(input("Masukkan Nilai UAS\t: "))                                    
        nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)              
        dataMhs[nama]= nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir                         
        print("\nData Berhasil Ditambahkan!")
````

saya juga melakukan percabangan if (elif) untuk melaksanakan pilihan yang lain
````py
    elif (c.lower() == 'u'):                                                                    
        print('\nMengedit Data Mahasiswa')
        nama = input("Masukkan Nama: ")                                                         
        if nama in dataMhs.keys():                              
            nim= input("Masukkan NIM Baru\t: ")                              
            nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))                           
            nilaiUts= int(input("Masukkan Nilai UTS\t: "))                           
            nilaiUas= int(input("Masukkan Nilai UAS\t: "))                           
            nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)          
            dataMhs[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir                      
            print("\nData Berhasil Di Update!")
````

dan saya juga menggunakan else untuk apabila salah memasukan pilihan inputan
````py
    else:
        print("Pilih menu yang tersedia: ")                                                    
````

## Tampilan Visual code 

![Gambar 6](gambar/TampilanProgram1.png)

## Output

![Gambar 7](gambar/Output1.png)
