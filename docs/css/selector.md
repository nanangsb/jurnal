## CSS Cheat Sheet Selektor: Panduan Lengkap dan Mendalam

**Klasifikasi Selektor:**

**1. Tipe Selektor:**

* **Menargetkan elemen berdasarkan tag HTML:**
    * `h1, h2, p, a, img` - Memilih semua heading, paragraf, tautan, dan gambar.
    * `div.content p` - Memilih semua paragraf di dalam div dengan kelas "content".
* **Contoh:**
    * `h1 { color: red; }` - Mengubah warna semua heading menjadi merah.
    * `p.small { font-size: 12px; }` - Memperkecil ukuran font semua paragraf dengan kelas "small".

**2. Kelas Selektor:**

* **Memilih elemen dengan kelas tertentu:**
    * `.class-name` - Memilih semua elemen dengan kelas `class-name`.
    * `.button:hover { background-color: green; }` - Mengubah warna latar belakang elemen dengan kelas "button" menjadi hijau saat di-hover.
* **Contoh:**
    * `.button { background-color: blue; }` - Memberikan warna biru kepada semua elemen dengan kelas "button".
    * `.card img { border-radius: 5px; }` - Memberikan radius border 5px kepada semua gambar di dalam elemen dengan kelas "card".

**3. ID Selektor:**

* **Memilih elemen dengan ID unik:**
    * `#id-name` - Memilih elemen dengan ID `id-name`.
    * `#main-content { width: 800px; }` - Mengatur lebar elemen dengan ID "main-content" menjadi 800px.
* **Contoh:**
    * `#header { background-color: #f0f0f0; }` - Memberikan warna latar belakang #f0f0f0 kepada elemen dengan ID "header".
    * `#footer a { color: white; }` - Mengubah warna semua tautan di dalam elemen dengan ID "footer" menjadi putih.

**4. Kombinator Selektor:**

* **Memilih elemen berdasarkan hubungannya dengan elemen lain:**
    * **Anak:** `parent > child` - Memilih elemen `child` yang merupakan anak langsung dari elemen `parent`.
    * **Keturunan:** `parent descendant` - Memilih semua elemen `descendant` di dalam elemen `parent`.
    * **Saudara:** `parent > child1 + child2` - Memilih elemen `child2` yang merupakan saudara langsung setelah elemen `child1` di dalam elemen `parent`.
* **Contoh:**
    * `.container > p { font-size: 16px; }` - Mengatur ukuran font semua paragraf yang merupakan anak langsung dari elemen dengan kelas "container" menjadi 16px.
    * `#main-content h2 { margin-top: 20px; }` - Memberikan margin atas 20px kepada semua heading 2 di dalam elemen dengan ID "main-content".
    * `.list-item:hover + .list-item { background-color: #ddd; }` - Mengubah warna latar belakang elemen "list-item" menjadi #ddd saat elemen "list-item" sebelumnya di-hover.

**5. Universal Selektor:**

* **Memilih semua elemen:**
    * `*` - Memilih semua elemen di halaman web.
* **Contoh:**
    * `* { margin: 0; padding: 0; }` - Menghapus margin dan padding semua elemen di halaman web.
    * `*:hover { cursor: pointer; }` - Mengubah kursor menjadi pointer saat meng-hover semua elemen di halaman web.

**6. Pseudo-kelas Selektor:**

* **Memilih elemen berdasarkan keadaan:**
    * `:hover` - Memilih elemen saat di-hover.
    * `:focus` - Memilih elemen saat difokuskan.
    * `:active` - Memilih elemen saat diklik.
* **Contoh:**
    * `a:hover { text-decoration: underline; }` - Memberikan garis bawah kepada semua tautan saat di-hover.
    * `input:focus { border-color: blue; }` - Mengubah warna border input menjadi biru saat difokuskan.

**7. Pseudo-elemen Selektor:**

* **Memilih bagian tertentu dari elemen:**
    * `::first-line` - Memilih baris pertama teks di dalam elemen.
    * `::before` - Menambahkan konten sebelum elemen.
    * `::after` - Menambahkan konten setelah elemen.
* **Contoh:**
    * `h1::first-line { text-transform: uppercase; }` - Mengubah semua huruf pertama di baris pertama heading 1 menjadi huruf besar.
    * `.button::before { content: ">"; }` - Menambahkan simbol ">" sebelum semua elemen dengan kelas "button".
    * `p::after { content: " "; }` - Menambahkan spasi setelah semua paragraf.

**8. Atribut Selektor:**

* **Memilih elemen berdasarkan atribut:**
    * `[attribute]` - Memilih elemen dengan atribut `attribute`.
    * `[attribute=value]` - Memilih elemen dengan atribut `attribute` dan nilai `value`.
    * `[attribute^=value]` - Memilih elemen dengan atribut `attribute` yang dimulai dengan nilai `value`.
    * `[attribute$=value]` - Memilih elemen dengan atribut `attribute` yang diakhiri dengan nilai `value`.
    * `[attribute*=value]` - Memilih elemen dengan atribut `attribute` yang mengandung nilai `value`.
* **Contoh:**
    * `img[alt]` - Memilih semua gambar dengan alt text.
    * `a[href^="https://"]` - Memilih semua tautan yang dimulai dengan "https://".
    * `input[type=radio]` - Memilih semua elemen input dengan type radio.
    * `[data-id*="123"]` - Memilih semua elemen dengan atribut `data-id` yang mengandung nilai "123".

**9. Kombinasi Selektor:**

* **Menggabungkan beberapa selektor untuk memilih elemen yang lebih spesifik:**
    * `selector1, selector2` - Memilih semua elemen yang cocok dengan `selector1` atau `selector2`.
    * `selector1 selector2` - Memilih semua elemen yang cocok dengan `selector1` dan `selector2`.
* **Contoh:**
    * `h1, h2 { color: red; }` - Mengubah warna semua heading 1 dan 2 menjadi merah.
    * `.container p.small { font-size: 12px; }` - Memperkecil ukuran font semua paragraf dengan kelas "small" di dalam elemen dengan kelas "container".

**10. Penjelasan Tambahan:**

* Urutan selektor penting. Selektor yang lebih spesifik akan diutamakan.
* Gunakan !important untuk memaksakan gaya pada elemen meskipun ada selektor yang lebih spesifik.
* Gunakan browser developer tools untuk melihat dan menguji selektor.

**Sumber Daya:**

* CSS Selectors Cheat Sheet: [https://www.w3schools.com/css/css_selectors.asp](https://www.w3schools.com/css/css_selectors.asp)
* CSS Selectors Tutorial: [https://www.freecodecamp.org/news/css-selectors-cheat-sheet/](https://www.freecodecamp.org/news/css-selectors-cheat-sheet/)
* CSS Selectors Reference: [https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)

**Catatan:**

* Cheat sheet ini hanya memuat informasi dasar tentang CSS Selektor.
* Untuk mempelajari lebih lanjut, silakan merujuk ke sumber daya yang disediakan.

**Semoga bermanfaat!**
