# labpy08

## PRAKTIKUM 8
### SOAL :

     Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:

     Method tambah() untuk menambah data
     Method tampilkan() untuk menampilkan data
     Method hapus(nama) untuk menghapus data berdasarkan nama
     Method ubah(nama) untuk mengubah data berdasarkan nama
     Buat diagram class, flowchart dan penjelasan programnya pada README.md.

### PENJELASAN :
- Buatlah dictionary yang akan diinput dengan data

      data = {}
      
- Membuat perulangan dan keterangan untuk pilihan menu

      while True:
        c = input("\n(L)ihat, (T)ambah, (U)bah), (H)apus, (C)ari, (K)eluar: ")
        
- Menambahkan data yang akan diinput kemudian masuk ke dalam dictionary

      if c.lower() == 't':
        print("Tambah Data")
        nama = input("Nama\t\t: ")
        nim = int(input("NIM\t\t: "))
        uts = int(input("Nilai UTS\t: "))
        uas = int(input("Nilai UAS\t: "))
        tugas = int(input("Nilai Tugas\t: "))
        akhir = tugas*30/100 + uts*35/100 + uas*35/100
        data[nama] = nim, uts, uas, tugas, akhir
        
### OUTPUT 

- Menambahkan data

      ![menambahkan data](https://user-images.githubusercontent.com/92702411/148877866-9fa1c7f7-e0a4-4c8c-9544-6e1baa6e88a8.png)
     
- Menampilkan data

      ![menampilkan data](https://user-images.githubusercontent.com/92702411/148877993-3509f703-6876-4224-9a26-1207e11f7204.png)
      
- Mengubah data
          
      ![mengubah data](https://user-images.githubusercontent.com/92702411/148878191-8bff4cff-6d51-4436-b36b-e3ed5e9a3ca7.png)

- Menghapus data

      ![menghapus data](https://user-images.githubusercontent.com/92702411/148878292-058aff5d-6100-4840-b7cc-14ef56adfed9.png)

- Jika sudah selesai input, pilih menu 'K' untuk memberhentikan program

      ![memberhentikan data](https://user-images.githubusercontent.com/92702411/148878504-93c4bf3a-c002-40a7-b4a4-09df3a8bcf6c.png)
