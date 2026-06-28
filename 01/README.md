./target{"txt"}
.#
** Struct
1) Variables
   1. [X] Penjelasan singkat mengenai variables (variables terdiri dari apa saja)
   2. [X] Tentang Scopes dan tempat penyimpanan Variables
2) Pointer
   1. [ ]  Apa itu pointer
   2. [ ]  Bagaimana Pointer Bekerja + Dereference
   3. [ ]  Apa saja yang disimpan dalam pointer
   4. [ ]  void*
}
.#

** Scripts
./title{
Speedrun Ngejelasin apa itu variabel dan pointer
}
mulai!
./part{.num=1, title="variables"}
Variables adalah konsep dasar dari pemograman yang merupakan konsep abstrak dari penyimpanan dengan label yang digunakan oleh
programmer untuk mengakses suatu data.

variables itu sendiri terdiri dari 4 Komponen: alamat memory, data, tipe data, dan nama simbolik.
1) jadi yang pertama nama simboli, nah... nama simbolik itu sendiri sebenarnya tidak pernah digunakan seutuhnya oleh compiler dan akan digantikan menjadi alamat memori
   sehingga nama simbolik ini hanya digunakan oleh manusia untuk bisa mengakses memori dengan nama yang baik
2) lalu ada tipe data, tipe data  ada untuk memberitahu compiler bagaimana data tersebut harus diolah. programmer biasanya yang akan menentukan tipe data apa yang
   akan digunakan, tapi ada beberapa bahasa bersifat dynamic typed language seperti python yang mana interpreter dari python sendiri yang menentukan tipe datanya
3) lalu data adalah nilai yang di simpan pada blok memori tersebut, data di komputer dapat di definisikan sebagai
4) dan terakhir alamat memory yaitu alamat dari memory dimana data tersebut disimpan. info tambahan adalah tempat dimana data disimpan tidak selalu sama dengan sebelumnya,
   sehingga alamat memory sangat dibutuhkan.

variables itu sendiri juga memiliki scopes. Scopes itu adalah region / area dimana variables itu dapat dibaca dimana  yang  paling umum ada dua yaitu
local scope dan global scope. local scope memungkinkan variabel hanya bisa dibaca dan digunakan di satu tempat seperti fungsi ataupun block, sedangkan
global scopes dapat diakses oleh seluruh sistem.

/.end{"part 1"}


./part{.num=2, .title="pointer"}
lalu pointer itu sendiri tidak lebih dan tidak bukan adalah variabel yang menyimpan alamat memori dan tipe data meski tipe datanya hanya disimpan di compiler saja,
pointer paling sering digunakan untuk melempar nilai dan untuk mengubah nilai - nilai itu dari proses ataupun fungsi lainnya. pada level hardware pointer juga
nilainya tidak lebih adalah angka yang biasanya ditampung dengan 64bit memori. Pointer itu juga dapat dilakukan operasi aritmatika yaitu dengan menambahkan
ataupun menguranginya nilainya, hal tersebut akan berefek pada pindahnya panah pointer yang menunjuk ke memori berdasarkan ukuran dari tipe data pointer tersebut

selain itu, salah satu fitur yang paling sering digunakan dari pointer adalah void pointer. void pointer tidak lebih hanyalah pointer yang tidak
menyertakan tipe datanya, sehingga compiler tidak bisa medereference karena compiler tidak mengetahui bagaimana caranya mengolah nilai yang ada
di pointer tersebut. kelebihannya adalah karena ini tidak perlu menyertakan tipe data, maka semua pointer ke segala jenis tipe data dapat di
cast dan diubah menjadi void pointer sehingga fungsi dapat menerima nilai dengan beragam jenis tipe data. tentunya juga dibutuhkan operasi
casting lagi untuk mengembalikan void pointer menjadi tipe data yang di inginkan

/.end{"part 2"}

