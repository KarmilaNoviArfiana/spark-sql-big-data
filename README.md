# SPARK

Nama   : Karmila Novi Arfiana

Kelas  : TI - 3C

NIM  : 2041720073

Absen : 09

## Pertanyaan Praktikum

Jelaskan masing-masing maksud kode berikut sesuai nomor kodenya pada laporan praktikum Anda!

### **mylist, myschema**

Kode ini digunakan untuk list dan scema awal yang digunakan untuk membuat dataframe


### **spark.createDataFrame**

pada kode ini digunakan untuk membuat DataFrame dari RDD, list, atau pandas.DataFrame. Contohnya :

1. Jika skemanya hanya berupa daftar nama kolom, tipe data setiap kolom akan secara otomatis disimpulkan dari data.
2. Jika tidak ada skema yang disediakan, Spark akan mencoba menyimpulkan skema (nama dan tipe kolom) dari data yang diberikan. Data harus berupa RDD dari Baris, bernama tuple, atau dict

### **parallelize, toDF**

parallelize digunakan untuk membuat RDD dari kumpulan list. Sedangkan toDF digunakan untuk mengembalikan DataFrame baru dan mengubah Dataset menjadi DataFrame.

### **hadoop, fs, put**

- Hadoop : sebuah framework open-source untuk menyimpan dan memproses data besar secara terdistribusi.
- fs : menyediakan akses ke berbagai sistem file termasuk Hadoop Distributed File System (HDFS) dan sistem file lokal.
- put : sebuah operasi untuk mengunggah file atau objek dari mesin lokal atau virtual ke sistem penyimpanan objek pada PySpark.

### **pyspark.sql, SQLContext, createOrReplaceTempView, show**

- pyspark.sql : package pada Apache Spark yang digunakan untuk mengakses data terstruktur menggunakan SQL dan DataFrame API pada lingkungan pemrograman Python.
- SQLContext : digunakan untuk mengakses data terstruktur menggunakan SQL pada lingkungan pemrograman Scala, Java, dan Python.
- createOrReplaceTempView : Membuat atau mengganti tampilan sementara lokal dengan DataFrame ini.
- show : Mencetak n baris pertama ke konsol.


### **textFile, map, lambda, strip, StructField, StringType**

- textFile : digunakan untuk membaca file teks yang tersimpan di HDFS, S3, dan sistem file lainnya yang dapat diakses oleh Hadoop.
- map : digunakan untuk memodifikasi setiap elemen RDD atau DataFrame dengan fungsi transformasi (lambda) dan menghasilkan RDD baru. 
- strip : digunakan untuk membersihkan atau menghilangkan karakter whitespace pada data yang dibaca dari suatu file.
- StructField : adalah representasi dari sebuah field di StructType. StructField terdiri dari tiga komponen yaitu, nama (sebagai string), tipe data (Tipe Data), dan nullable (boolean), dimana nama field adalah nama dari StructField tersebut.
- StringType : digunakan untuk merepresentasikan nilai string.

### **spark.read.format, jdbc, options, load**

- spark.read.format : digunakan untuk membaca data dari berbagai sumber data seperti file CSV, JSON, Parquet, Avro, dan lain-lain. 
- jdbc : digunakan untuk membaca dan menulis data dari database menggunakan JDBC (Java Database Connectivity).
- options : digunakan untuk menentukan opsi konfigurasi saat membaca atau menulis data dari atau ke sumber eksternal.
- load : digunakan untuk memuat data ke dalam DataFrame dengan format tertentu, seperti CSV, JSON, parquet, atau ORC.

### **show**

show di Apache Spark digunakan untuk menampilkan data dari DataFrame secara tabular. DataFrame adalah struktur data yang mirip dengan tabel dalam database relasional. Metode show secara default menampilkan 20 baris pertama dari DataFrame.

### **collect, rdd, take**

- collect : digunakan untuk mengambil seluruh data dari DataFrame dan dikumpulkan dalam bentuk Python list. Namun, metode ini dapat menyebabkan overhead yang besar terutama jika data yang diolah sangat besar.
- rdd : digunakan untuk kumpulan data yang terdistribusi di seluruh node dalam sebuah cluster, yang dapat diproses secara terpisah dan paralel.
- take : digunakan untuk mengambil sejumlah baris dari RDD atau DataFrame dan mengembalikan hasilnya ke driver node dalam bentuk Python list.

### **makeRDD, Seq, createDataset**

- makeRDD : digunakan untuk membuat RDD baru dari data yang sudah ada di dalam memori, seperti list, tuple, atau array. Dengan menggunakan makeRDD, pengguna dapat membuat RDD secara eksplisit dari data yang disediakan.
- Seq : tipe data di Scala yang merepresentasikan sebuah urutan dari elemen-elemen yang dapat diakses secara berurutan. Pada Spark, Seq sering digunakan sebagai parameter input untuk metode yang memerlukan sebuah kumpulan data atau sekumpulan nilai. Seq juga dapat digunakan untuk membuat kumpulan data dalam bentuk RDD.
- createDataset : digunakan untuk membuat sebuah Dataset, yaitu struktur data yang mirip dengan DataFrame.

### **filter**

Filter digunakan untuk melakukan penyaringan pada Dataset atau DataFrame dengan kriteria tertentu. Metode ini menerima ekspresi boolean sebagai parameter dan mengembalikan Dataset atau DataFrame yang hanya berisi baris yang memenuhi kriteria tersebut.

### **as, toDF, first**

- as : digunakan untuk memberikan alias (nama lain) pada sebuah kolom dalam sebuah DataFrame atau Dataset. Alias ini bisa berguna untuk memberikan nama yang lebih deskriptif dan mudah dipahami pada kolom-kolom yang dihasilkan dari operasi-operasi transformasi pada DataFrame.
- toDF : digunakan untuk mengubah sebuah RDD (Resilient Distributed Dataset) menjadi sebuah DataFrame. toDF menerima parameter berupa nama-nama kolom untuk DataFrame yang dihasilkan, atau bisa juga tidak memiliki parameter untuk menghasilkan DataFrame dengan kolom-kolom default ("_1", "_2", dst).
- first : digunakan untuk mengembalikan elemen pertama dari RDD. Metode ini mengambil satu elemen pertama dari RDD dan mengembalikannya ke driver program. Metode first sangat berguna ketika pengguna ingin melihat elemen pertama dari RDD, seperti ketika ingin memeriksa struktur dari data yang sedang diolah.

### **listDatabases, listTables, listFunctions, isCached, select**

- listDatabases : Mengembalikan daftar database yang tersedia di semua sesi.
- listTables : Mengembalikan daftar tabel/tampilan dalam database yang ditentukan.
- listFunctions : Mengembalikan daftar fungsi yang terdaftar di database yang ditentukan.
- isCached : Mengembalikan nilai true jika tabel saat ini di-cache dalam memori.
- select : Memproyeksikan sekumpulan ekspresi dan mengembalikan DataFrame baru.

### **Read, text**

- Read : digunakan untuk menyesuaikan cara data dibaca dari source data.
- text : digunakan untuk membaca file teks dan mengonversinya menjadi sebuah DataFrame.

### **load, json, format, printSchema**

- load : digunakan untuk memuat data dari sumber data dan mengembalikannya dalam bentuk DataFrame. 
- json : digunakan untuk membaca file JSON ke dalam Spark DataFrame. 
- format : digunakan untuk memuat file atau memformat data yang berasal dari sumber data dengan tipe data tertentu. 
- printSchema : digunakan untuk mencetak skema DataFrame dalam format pohon.

### **write, save**

- write : digunakan untuk menyimpan konten DataFrame yang bukan streaming ke penyimpanan eksternal. 
- save : digunakan untuk menyimpan konten DataFrame ke sumber data. Metode save dapat digunakan untuk menyimpan DataFrame dalam berbagai format, seperti CSV, JSON, atau Parquet.

### **parquet**

parquet digunakan untuk menyimpan data secara kolomar dalam bentuk kompresi, yang terdiri dari beberapa baris dan kolom.

### **Options, inferSchema, csv, header, codec**

- Options: digunakan untuk menyesuaikan atau memberikan opsi pada bagaimana data akan dibaca dari sumbernya.
- inferSchema: merupakan alternatif dari fungsi schema yang dapat menyesuaikan tipe data kolom pada file CSV dengan lebih cepat.
- csv: digunakan untuk memuat file CSV dan mengembalikan hasilnya sebagai DataFrame.
- header: merupakan opsi yang digunakan jika file CSV memiliki header, sehingga baris pertama akan digunakan sebagai nama kolom.
- codec: opsi ini digunakan untuk menentukan codec kompresi yang akan digunakan pada output. Beberapa codec yang didukung adalah gzip, snappy, dan bzip2.