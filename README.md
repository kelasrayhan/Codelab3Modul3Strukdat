Nama : Rayhan Rizky Widi Ananta
NIM : 202210370311470
Prak Strukdat G


Penjelasan Codelab 1 :::

 Stack s = new Stack();

        System.out.println(s.empty());

        s.push("Bebek");
        s.push("Angsa");

        s.push("Kuda");
        s.push("Buaya");

        s.push("Tikus");

        System.out.println(s.empty());

        System.out.println("Peek: " + s.peek());
        System.out.println("Animals: " + s);

        s.pop();
        s.pop();

        System.out.println("Animals: " + s);
        System.out.println("Position of Kuda: " + s.search("Kuda"));


============ Penjelasan Codelab 1 ==============


Kita masukan/push semua data ini :
  `     s.push("Bebek");
        s.push("Angsa");

        s.push("Kuda");
        s.push("Buaya");

        s.push("Tikus");

        Yang berarti outputnya
        Animals: [Bebek, Angsa, Kuda, Buaya, Tikus]


        Kemudian kita tampilkan Peek nya, disini peeknya adalah "Tikus", dan Animals nya masih belum di ubah

        System.out.println("Peek: " + s.peek());
        System.out.println("Animals: " + s);

        Output :
        Peek: Tikus
        Animals: [Bebek, Angsa, Kuda, Buaya, Tikus]

    
        Kemudian disini kita pop atau kita keluarkan 2 dari atas yaitu  Buaya, Tikus, kemudian di cetak posisi kuda saat ini, dan posisi kuda itu berada paling atas/first

        s.pop();
        s.pop();
        System.out.println("Animals: " + s);
        System.out.println("Position of Kuda: " + s.search("Kuda"));

        Outputnya :  Animals: [Bebek, Angsa, Kuda] 
                     Position of Kuda: 1


    Penjelasan Singkat : Pada langkah pertama, data dimasukkan ke dalam stack, seperti menumpuk piring, dengan data terakhir di atas. Operasi peek hanya melihat data paling atas tanpa mengubahnya, seperti melihat piring paling atas tanpa mengangkatnya. Dua operasi pop kemudian menghapus dua data paling atas, seperti mengangkat dua piring paling atas. Ketika mencari data "Kuda" setelah dua pop, data tersebut tidak ditemukan karena sudah dihapus. Posisi data dalam stack dapat berubah setelah operasi pop, seperti urutan piring di tumpukan setelah beberapa piring diangkat.


============ Penjelasan Codelab 2 ==============


    Membuat Objek Queue: Pertama, kita membuat objek Queue dengan menggunakan kelas LinkedList. Kita inisialisasi dengan tipe data String.

    Queue<String> q = new LinkedList<>();
    Menambahkan Elemen ke dalam Queue: Selanjutnya, kita menambahkan beberapa elemen ke dalam queue menggunakan metode add().

    q.add("Bebek");
    q.add("Angsa");
    q.add("Kuda");
    q.add("Buaya");
    q.add("Tikus");

    Melihat Elemen Teratas (Peek): Kita dapat melihat elemen yang berada di depan queue tanpa menghapusnya menggunakan metode peek().

    System.out.println("Peek: " + q.peek());
    Mencetak Seluruh Elemen Queue: Setelah menambahkan elemen, kita mencetak seluruh isi queue.

    System.out.println("Animals: " + q);
    Menghapus Elemen dari Queue (Poll): Kita menghapus dua elemen pertama dari queue menggunakan metode poll().

    q.poll();
    q.poll();
    Cetak Elemen Setelah Penghapusan: Terakhir, kita mencetak isi queue setelah menghapus dua elemen.

    System.out.println("Animals: " + q);
    Dengan demikian, hasil dari program ini akan mencetak elemen yang ditambahkan ke dalam queue serta menunjukkan operasi peek dan poll yang dilakukan terhadap queue tersebut.

    Penjelasan Singkat : Kode ini membuat antrian "Animals" dengan menggunakan linked list. Kita masukkan data hewan ("Bebek", "Angsa", dll.) ke dalam antrian seperti orang yang mengantri.
    peek() seperti melihat orang di depan antrian tanpa mengeluarkannya. System.out.println("Animals: " + q) menunjukkan semua orang di antrian. poll() seperti mengeluarkan dua orang pertama dari antrian. System.out.println("Animals: " + q) menunjukkan antrian setelah dua orang dikeluarkan.