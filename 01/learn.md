# [GNU Variables](https://www.gnu.org/software/c-intro-and-ref/manual/html_node/Variables.html)
eklarasi variables teridiri dari hal berikut
__keywords basetype symbolic_names;__

dan apabila langsung bersama definition:
__keywords basetype symbolic_names = init;__

di c keywords dan basetype terserah di taruh di urutan mana, bisa __basetype__ duluan lalu __keywords__, sebaliknya, atau bahkan keywords
ditengah dari __basetype__.

selain itu juga, __basetype__ itu sendiri memiliki **type qualifiers** yang mana **type qualifiers** terdiri dari __const__, __register__,
__volatile__, dan lainnya

# [Wikipedia](https://en.wikipedia.org/wiki/Variable_(high-level_programming_language))
variables adalah konsep dasar high level dari pemograman
yang merupakan konsep abstrak dari penyimpanan yang digunakan oleh komputer untuk menyimpan nilai, tipe data, dan nama simbolik.

nama simbolik hanya digunakan oleh programmer itu sendiri untuk bisa secara spesifik mengakses lokasi data atau menunjuk data secara spesifik.
untuk komputer itu sendiri, compiler akan menghapus nama simbolik itu dan menggantinya dengan alamat memori dan tipe data tersebut.

salah satu alasan mengapa variable itu penting dikarenakan di setiap  kali run suatu program, alamat data yang disimpan tidak selalu di tempat
yang sama, variables memberikan kemudahan untuk bisa mengakses alamat data tersebut meski alamatnya berubah di setiap run

lalu variables itu sendiri tinggal di area yang bernama scopes, setiap variables itu akan hidup mengikuti scopes dimana ketika scopes itu
dihapus maka variables tersebut juga akan ikut mati bersama scopes. ada dua jenis scopes yaitu local scopes dan global scopes, yang mana
variable yang hanya dapat dilihat dalam suatu stack / scope yang sama dijuluki local scopes sedangkan variable yang dapat dilihat oleh seluruh
fungsi atau dapat dilihat di seluruh bagian dari program dijuluki global scopes, tentu masih ada beberapa lagi yang dapat dijelaskan seperti
dynamic scopes dan file scopes

notes tambahan:
untuk semua variables yang masa hidup nilai aslinya melebihi masa hidup dari scopes tersebut dan bahasa pemogramannya masih manual memory
allocation, maka hampir mustahil untuk mengfree nilai variables tersebut dikarenakan variables yang menjadi reference / pointer ke memory itu
sudah tidak ada sehingga fungsi free tidak dapat dipanggil / tidak diketahui alamat memory mana yang tidak akan digunakan lagi

di bahasa statis, variables mengikuti types berdasarkan bagaimana types itu dijelaskan, sedangkan di dynamic typed tipe data ditentukan oleh
nilai yang diterima

# [Understanding Variables in Programming](https://medium.com/@tick-to-trade/understanding-variables-in-programming-3a1ae74feec2)
apabila programmer harus membaca / menunjuk data secara manual dengan memberikan nilai pointer ke memory adress, pemograman akan sangat
melelahkan, terutama fakta bahwa setiap kali program dijalankan posisi memori mereka selalu berbeda. dari masalah tersebut muncullah variables
yang menjadi jembatan antara manusia dan komputer itu sendiri. variables memberikan manusia label dalam tulisan nama simbolik yang akan selalu
menunjuk pada alamat memori yang selalu tepat secara relatif pada memori program


