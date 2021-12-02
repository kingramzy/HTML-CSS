### HTML Tag Label

## Contoh

tiga tombol radio dengan label:

```html
<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML" />
  <label for="html">HTML</label><br />
  <input type="radio" id="css" name="fav_language" value="CSS" />
  <label for="css">CSS</label><br />
  <input type="radio" id="javascript" name="fav_language" value="JavaScript" />
  <label for="javascript">JavaScript</label><br /><br />
  <input type="submit" value="Submit" />
</form>
```

## Definisi dan Penggunaan

Tag <label> mendefinisikan label untuk beberapa elemen:

- <input type="checkbox">
- <input type="color">
- <input type="date">
- <input type="datetime-local">
- <input type="email">
- <input type="file">
- <input type="month">
- <input type="number">
- <input type="password">
- <input type="radio">
- <input type="range">
- <input type="search">
- <input type="tel">
- <input type="text">
- <input type="time">
- <input type="url">
- <input type="week">
- <meter>
- <progress>
- <select>
- <textarea>

Penggunaan label yang tepat dengan elemen-elemen di atas akan bermanfaat jika:

- Pengguna pembaca layar (akan membacakan label dengan keras, saat pengguna fokus pada elemen)
- Pengguna yang mengalami kesulitan mengeklik wilayah yang sangat kecil (seperti kotak centang) - karena ketika pengguna mengeklik teks di dalam elemen <label>, ini akan mengaktifkan input (ini meningkatkan area klik).

## Tips dan Catatan

Tip: Atribut for dari <label> harus sama dengan atribut id dari element terkait untuk mengikatnya bersama. Label juga dapat ke elemen dengan menempatkan elemen di dalam elemen <label>.

## Browser Pendukung

| Elemen | Google Chrome | Internet Explorer/Edge | Mozilla Firefox | Safari | Opera |
| :----: | :-----------: | :--------------------: | :-------------: | :----: | :---: |
| Label  |      Yes      |          Yes           |       Yes       |  Yes   |  Yes  |

## Atribut

| Atribut |   Nilai    |                            Deskripsi                            |
| :-----: | :--------: | :-------------------------------------------------------------: |
|   for   | element_id | Menentukan id dari elemen formulir yang harus diikat oleh label |
|  form   |  form_id   |                  Menentukan bentuk label milik                  |

## Atribut Global HTML

Tag <link> juga masuk dalam kategori tabel Atribut Global HTML

## Atribut Event HTML

Tag <link> juga masuk dalam kategori tabel Atribut Event HTML

## Pengaturan CSS Bawaan

Sebagian besar browser akan menampilkan elemen <label> dengan nilai default berikut:

```css
label {
  cursor: default;
}
```

Sumber : https://www.w3schools.com/tags/tag_label.asp
