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
