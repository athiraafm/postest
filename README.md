# postest
username = "Athira"
nim = "2309116010"
kelas = "A"

def mulai():
    print("Masukkan Data")
    user = str(input("Nama : "))
    nm = str(input("NIM : "))
    kls = str(input("Kelas : "))
    if user == username and nm == nim and kls == kelas:
        print("""
                  +====================+
                  |   Selamat Datang!  |
                  +====================+
                  """)
        while True:
            print("""
                  +====================+
                  |    BANGUN RUANG    |
                  +====================+
                  | 1 | Bola           |
                  | 2 | Tabung         |
                  | 3 | Limas Segitiga |
                  | 4 | Keluar         |
                  +====================+
                  """)
            pilih = input("Masukkan Pilihan: ")
            
            if pilih == "1":
                print("Menghitung Volume Bola")
                r = int(input("Masukkan Jari - Jari: "))
                lb = 4/3 * 22/7 * (r * r * r)
                print("Volume Bola adalah", lb)
            elif pilih == "2":
                print("Menghitung Volume Tabung")
                r = int(input("Masukkan Jari - Jari: "))
                t = int(input("Masukkan Tinggi Tabung: "))
                vt = 22/7 * r * r * t
                print("Volume Tabung adalah", vt)
            elif pilih == "3":
                print("Menghitung Volume Limas Segitiga")
                la = int(input("Masukkan Luas Alas: "))
                tl = int(input("Masukkan Tinggi Limas: "))
                vl = 1/3 * la * tl
                print("Volume Limas Segitiga adalah", vl)
            elif pilih == "4":
                print("Goodbye")
                break
            else:
                print("Pilihan tidak valid. Silakan pilih 1, 2, 3, atau 4.")
    else:
        print("""
              +====================================+
              |   kata yang anda masukkan salah,   |
              |        silahkan coba lagi          |
              +====================================+
              """)
        mulai()

mulai()
