### HTML SVG Graphics

SVG mendefinisikan grafik berbasis vektor dalam format XML.

## Apa itu SVG?

- SVG adalah singkatan dari Scalable Vector Graphics
- SVG digunakan untuk mendefinisikan grafik untuk Web
- SVG adalah rekomendasi W3C

## HTML Elemen SVG

Elemen HTML <svg> adalah container untuk grafik SVG.

SVG memiliki beberapa metode untuk menggambar jalur, kotak, lingkaran, teks, dan gambar grafik.

## Browser Pendukung

| Elemen | Google Chrome | Internet Explorer/Edge | Mozilla Firefox | Safari | Opera |
| :----: | :-----------: | :--------------------: | :-------------: | :----: | :---: |
|  SVG   |      Yes      |          Yes           |       Yes       |  Yes   |  Yes  |

### Lingkaran SVG

![Lingkaran](./LingkaranSVG.png)

## Contoh

```html
<!DOCTYPE html>
<html>
  <body>
    <svg width="100" height="100">
      <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
    </svg>
  </body>
</html>
```

### Persegi Panjang SVG

![Persegi](./PersegiPanjangSVG.png)

## Contoh

```html
<svg width="400" height="100">
  <rect width="400" height="100" style="fill:rgb(0,0,255);stroke-width:10;stroke:rgb(0,0,0)" />
</svg>
```

### Persegi Panjang Bulat SVG

![Persegi](./PersegiPanjangBulatSVG.png)

## Contoh

```html
<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150" style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
</svg>
```

### Bintang SVG

![Bintang](./BintangSVG.png)

## Contoh

```html
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198" style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
```

### Logo SVG

![Bintang](./LogoSVG.png)

## Contoh

```html
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
  Sorry, your browser does not support inline SVG.
</svg>
```

## Perbedaan SVG dan Canvas

- SVG adalah bahasa untuk menggambarkan grafik 2D dalam XML.
- Canvas menggambar grafik 2D, dengan cepat (dengan JavaScript).
- SVG berbasis XML, yang berarti bahwa setiap elemen tersedia dalam DOM SVG. Anda dapat melampirkan event handler JavaScript untuk sebuah elemen.
- Di SVG, setiap bentuk yang digambar diingat sebagai objek. Jika atribut objek SVG diubah, browser dapat merender ulang bentuk secara otomatis.
- Kanvas dirender piksel demi piksel. Di kanvas, setelah grafik digambar, itu dilupakan oleh browser. Jika posisinya harus diubah, seluruh pemandangan perlu digambar ulang, termasuk objek apa pun yang mungkin tertutup oleh grafik.

## Perbandingan Canva dan SVG

Tabel di bawah ini menunjukkan beberapa perbedaan penting antara Canvas dan SVG:

|                         Canvas                         |                                      SVG                                      |
| :----------------------------------------------------: | :---------------------------------------------------------------------------: |
|                  Tergantung Resolusi                   |                              Resolusi independen                              |
|         Tidak ada dukungan untuk event handler         |                            Mendukung event handler                            |
|          Kemampuan rendering teks yang buruk           |     Paling cocok untuk aplikasi dengan area rendering besar (Google Maps)     |
| Bisa menyimpan gambar dengan format file .png dan .jpg | Rendering lambat jika rumit (apa pun yang menggunakan DOM banyak akan lambat) |
|     Sangat cocok untuk game dengan grafis intensif     |                        Tidak cocok untuk aplikasi game                        |
