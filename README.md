## Praktikum 2 : CSS Dasar
### 1. CSS Internal
Internal CSS adalah kode CSS yang ditulis di dalam tag  `<style>`. Internal CSS juga dikenal dengan sebutan  _Embeded CSS_.

Tag  `<style>`  biasanya ditulis di dalam tag  `<head>`. Bisa juga ditulis di dalam  `<body>`, namun lebih banyak ditulis di dalam  `<head>`.

**Contoh pendeklarasian CSS Internal:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode2.PNG)

Terdapat tag `<style>` di dalam tag `<head>` dalam kode di atas.

**Hasilnya:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/ss2.PNG)

**Manfaat Internal CSS:**

-   Perubahan hanya terjadi pada 1 halaman
-   Class dan ID bisa digunakan oleh internal stylesheet
-   Tidak perlu meng-upload beberapa file karena HTML dan CSS bisa digunakan di file yang sama.

**Kekurangan menggunakan Internal CSS:**

-   Meningkatkan waktu akses website
-   Perubahan hanya terjadi pada 1 halaman – tidak efisien bila Anda ingin menggunakan CSS yang sama pada beberapa file.

### 2. Inline CSS
Inline CSS adalah kode CSS yang ditulis langsung pada atribut elemen HTML. Setiap elemen HTML memiliki atribut `style`, di sana lah inline CSS ditulis.

**Contoh pendeklarasian Inline CSS:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode3.PNG)

Dalam kode di atas, terdapat atribut `style` dalam tag `<p>`.

**Hasilnya:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/ss3.PNG)

**Manfaat Inline CSS:**

-   Berguna jika Anda ingin menguji dan melihat perubahan
-   Berguna untuk perbaikan cepat
-   Permintaan HTTP yang lebih kecil

**Kekurangan Inline CSS:**

-   Inline CSS harus diterapkan pada setiap elemen

## 3. CSS Eksternal
Eksternal CSS adalah kode CSS yang ditulis terpisah dengan kode HTML. Eksternal CSS ditulis disebuah file khusus yang berekstensi `.css`.

Sebagai contoh, saya membuat sebuah file bernama `.css`. Berikut ini isi file `style_eksternal.css`

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode4b.PNG)

Untuk menggunakan CSS Eksternal dalam HTML, kita perlu mengimpornya dengan menggunakan tag `<link>` dan biasanya diletakkan setelah bagian `<head>`, seperti contoh di bawah ini:

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode4c.PNG)

Berikut ini penulisan HTML versi lengkapnya:

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode4a.PNG)

**Dan seperti ini hasilnya:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/ss4.PNG)

**Manfaat CSS eksternal:**

-   Ukuran file HTML menjadi lebih kecil dan strukturnya lebih rapi
-   Kecepatan loading menjadi lebih cepat
-   File CSS yang sama bisa digunakan di banyak halaman.

**Kekurangan CSS eksternal:**

-   Halaman belum tampil secara sempurna hingga file CSS selesai dipanggil.

## 4. CSS Selector
**Selektor** adalah kata kunci dan simbol yang digunakan pada CSS untuk menyeleksi atau memilih elemen HTML.

 **1. ID Selector**
 - ID selector menggunakan atribut `id` pada  HTML  untuk memilih elemen tertentu.
 - ID dari elemen bersifat unik dalam suatu laman, jadi ID selector digunakan untuk memilih satu elemen unik.
 -  ID Selector ditandai dengan tanda pagar `(#)` di depannya.

**2. Class Selector**
 - Class Selector adalah selektor yang memilih elemen berdasarkan nama class yang diberikan. 
 - Class Selector dibuat dengan tanda titik `(.)` di depannya.
 
 **Contoh ID dan Class Selector:**
 
 ![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode5.PNG)

**Hasilnya:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/ss5.PNG)

## Jawaban dari pertanyaan pada Praktikum 2
1. 
2. Perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}`:
 - Pada elemen `h1 {...}` merupakan salah satu elemen yang 
diletakkan pada tag `<style>` dan berada didalam tag `<head>`, dan merupakan contoh pendeklarasian CSS Internal.
 - Sedangkan, elemen `#intro h1 {...}`merupakan salah satu elemen dalam pendeklarasian ID Selector, dimana intro merupakan pembuka website sebelum masuk ke tampilan utama halaman website.
 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser?
 
 **Jawab:**
 
 - Deklarasi yang akan ditampilkan pada browser adalah **Inline CSS**. 
 - Penggunakan CSS Inline hanya sebatas pada kode markup HTML saja yang ingin dilakukan perubahan pada bagian tersebut secara langsung. Jadi tidak dibutuhkan kode CSS dengan struktur yang baku.
 
 - **Contoh:**
 
 Deklarasi CSS Internal, CSS Eksternal, dan Inline CSS.
 
 ![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode6.PNG)

File khusus berekstensi `.css` dalam deklarasi CSS Eksternal.

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode7.PNG)

**Dan hasilnya seperti berikut ini:**

![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/ss6.PNG)

terlihat bahwa yang ditampilkan dalam browser adalah deklarasi Inline CSS, seperti penggunaan property `font-family` dan `color`.

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?

**Jawab:**

 - Deklarasi yang akan ditampilkan pada browser adalah deklarasi **ID Selector**.
 - ID Selector ini merupakan selector untuk menentukan bagian yang hanya ada satu pada halaman dan juga menentukan style nya. Jadi selector ID ini tidak bisa dipanggil lebih dari satu. Jika ada dua, maka hanya bekerja pada bagian pertama saja.
 
 - **Contoh:**
 
 ![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode8.PNG)


![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode9.PNG)
 

 - **Hasilnya:**
 
 ![enter image description here](https://github.com/kameliacindy/Lab2Web/blob/main/img/kode9.PNG)

Semoga bermanfaat...

Nama	: Kamelia Cindy Astuti
NIM	: 311910104
Kelas	: TI. 19. A. 1
