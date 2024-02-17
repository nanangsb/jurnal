## CSS Cheat Sheet: Pseudo Selectors & Elements

**Pseudo Selectors:**

**1. Keadaan Elemen:**

* **:hover:** Saat elemen di-hover.
    * Contoh:
        * `a:hover { color: blue; text-decoration: underline; }` - Mengubah warna tautan menjadi biru dan menambahkan garis bawah saat di-hover.
        * `button:hover { background-color: #f0f0f0; }` - Mengubah warna background button menjadi #f0f0f0 saat di-hover.
* **:focus:** Saat elemen difokuskan.
    * Contoh:
        * `input:focus { border-color: red; outline: none; }` - Mengubah warna border input menjadi merah dan menghilangkan outline saat difokuskan.
        * `textarea:focus { font-size: 18px; }` - Memperbesar ukuran font textarea saat difokuskan.
* **:active:** Saat elemen diklik.
    * Contoh:
        * `.button:active { background-color: green; transform: scale(1.1); }` - Mengubah warna background button menjadi hijau dan memperbesarnya 1.1x saat diklik.
        * `a:active { color: orange; }` - Mengubah warna tautan menjadi orange saat diklik.
* **:visited:** Saat tautan telah dikunjungi.
    * Contoh:
        * `a:visited { color: purple; text-decoration: none; }` - Mengubah warna tautan yang telah dikunjungi menjadi ungu dan menghilangkan garis bawah.
        * `a:visited:hover { color: #666; }` - Mengubah warna tautan yang telah dikunjungi menjadi #666 saat di-hover.
* **:enabled:** Saat elemen dapat diinteraksikan.
    * Contoh:
        * `input:disabled { opacity: 0.5; cursor: not-allowed; }` - Mengurangi opacity input dan mengubah cursor menjadi not-allowed saat tidak dapat diinteraksikan.
        * `button:disabled { background-color: #ddd; }` - Mengubah warna background button menjadi #ddd saat tidak dapat diinteraksikan.
* **:disabled:** Saat elemen tidak dapat diinteraksikan.
    * Contoh:
        * `button:disabled { cursor: default; }` - Mengubah cursor menjadi default pada button yang tidak dapat diinteraksikan.
        * `select:disabled { opacity: 0.7; }` - Mengurangi opacity dropdown saat tidak dapat diinteraksikan.

**2. Posisi Elemen:**

* **:first-child:** Elemen pertama di dalam parent.
    * Contoh:
        * `p:first-child { font-weight: bold; }` - Mempertebal font paragraf pertama di dalam parent.
        * `li:first-child { margin-top: 10px; }` - Memberikan margin atas 10px pada elemen list pertama di dalam parent.
* **:last-child:** Elemen terakhir di dalam parent.
    * Contoh:
        * `h3:last-child { margin-bottom: 0; }` - Menghilangkan margin bawah pada heading 3 terakhir di dalam parent.
        * `img:last-child { display: block; }` - Mengubah elemen gambar terakhir di dalam parent menjadi block element.
* **:nth-child(n):** Elemen ke-n di dalam parent.
    * Contoh:
        * `div:nth-child(2) { background-color: yellow; }` - Mengubah warna background elemen div ke-2 di dalam parent menjadi kuning.
        * `p:nth-child(even) { text-align: right; }` - Menyejajarkan teks paragraf ke kanan pada elemen genap di dalam parent.
* **:only-child:** Elemen tunggal di dalam parent.
    * Contoh:
        * `h1:only-child { text-align: center; }` - Menyejajarkan teks heading 1 tunggal di dalam parent ke tengah.
        * `.card:only-child { margin: 0 auto; }` - Memberikan margin 0 auto pada elemen card tunggal di dalam parent.

**3. Konten Elemen:**

* **:empty:** Elemen tidak memiliki konten.
    * Contoh:
        * `p:empty { display: none; }` - Menyembunyikan paragraf yang tidak memiliki konten.
        * `span:empty { border: 1px solid red; }` - Memberikan border merah pada elemen span yang tidak memiliki konten.

* **:not(selector):** Elemen yang tidak sesuai dengan selector.
    * Contoh:
        * `p:not(.small) { font-size: 16px; }` - Mengatur ukuran font semua paragraf yang tidak memiliki class "small" menjadi 16px.
        * `a:not(:visited) { color: blue; }` - Mengubah warna tautan yang belum dikunjungi menjadi biru.
* **:matches(selector):** Elemen yang sesuai dengan selector.
    * Contoh:
        * `.button:matches(:hover, :active) { background-color: green; }` - Mengubah warna background button menjadi hijau saat di-hover atau diklik.
        * `input:matches([type="radio"]) { margin-right: 10px; }` - Memberikan margin kanan 10px pada semua elemen input dengan type radio.

**Pseudo Elements:**

* **::before:** Menambahkan konten sebelum elemen.
    * Contoh:
        * `h1::before { content: "• "; }` - Menambahkan simbol "•" sebelum semua heading 1.
        * `.button::before { content: ">"; }` - Menambahkan simbol ">" sebelum semua elemen dengan class "button".
* **::after:** Menambahkan konten setelah elemen.
    * Contoh:
        * `p::after { content: " "; }` - Menambahkan spasi setelah semua paragraf.
        * `blockquote::after { content: " — "; }` - Menambahkan simbol " — " setelah semua blockquote.
* **::first-line:** Memilih baris pertama teks di dalam elemen.
    * Contoh:
        * `h2::first-line { text-transform: uppercase; }` - Mengubah semua huruf pertama di baris pertama heading 2 menjadi huruf besar.
        * `p::first-line { font-size: 18px; }` - Memperbesar ukuran font baris pertama pada semua paragraf.
* **::selection:** Gaya saat teks di elemen diseleksi.
    * Contoh:
        * `::selection { background-color: yellow; color: black; }` - Mengubah warna background teks yang diseleksi menjadi kuning dan warna teks menjadi hitam.
        * `p::selection { font-weight: bold; }` - Mempertebal font teks yang diseleksi di dalam paragraf.

**Catatan:**

* Gunakan browser developer tools untuk melihat dan menguji pseudo selectors & elements.
* Kombinasikan pseudo selectors & elements untuk menargetkan elemen dengan lebih spesifik.
* Gunakan !important untuk memaksakan gaya pada elemen meskipun ada pseudo selectors & elements yang lebih spesifik.

**Semoga bermanfaat!**

[^1]:
CSS Selectors Cheat Sheet: [https://www.w3schools.com/css/css_selectors.asp](https://www.w3schools.com/css/css_selectors.asp)
    
[^2]:
CSS Selectors Tutorial: [https://www.freecodecamp.org/news/css-selectors-cheat-sheet/](https://www.freecodecamp.org/news/css-selectors-cheat-sheet/)

[^3]:
CSS Selectors Reference: [https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)