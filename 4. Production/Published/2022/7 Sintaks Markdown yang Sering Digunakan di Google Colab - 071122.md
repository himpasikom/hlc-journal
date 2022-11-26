Related : [[Engineering for Researchers - 1st]]
Tag : #markdown #googleColab
Source : [article link](somelink)
Author : [[MKom 21 - Muhammad Ihsan]]

Google Colab memiliki 2 jenis format penulisan, kode dan teks. Teks pada Google Colab memiliki format berupa **_Markdown_**. Pada artikel ini akan dibahas terkait perintah-perintah yang mungkin akan sering kita gunakan ketika bekerja dengan teks pada Google Colab. Pada artikel ini, akan dibahas beberapa _command_ yang kemungkinan akan berguna dan sering digunakan untuk mengatur dokumen di Google Colab.

## 1. Header

Pengaturan _header_ bisa membantu kita dalam menyusun dan melakukan navigasi di dalam notebook colab kita, terutama jika notebook yang kita tulis tersusun atas beberapa bagian. Untuk menandakan kata / kalimat sebagai _header_ di dalam dokumen maka kita cukup menambahkan tanda `#` di depan kata / kalimat yang diinginkan.

```
# Bagian 1
# Bagian 2
## Sub dari bagian 2
### Subbagian dari subbagian 2
# Bagian 3
```
Tampilan dari _markdown_ di atas adalah seperti gambar di bawah ini:
<img width="1145" alt="Jepretan Layar 2022-11-07 pukul 17 39 17" src="https://user-images.githubusercontent.com/62195104/200303140-f763bcd2-27a3-404a-bf6e-43620ef74c9d.png">

Bagian-bagian tersebut akan terlihat pada menu 'Daftar Isi', dengan ini kita dapat lebih mudah untuk bernavigasi di notebook yang kita buat. Dengan mengatur bagian-bagian di dalam notebook, kita dimungkinkan untuk dapat mengatur kode-kode yang ada dan memudahkan untuk dibaca ulang.

<img width="330" alt="Jepretan Layar 2022-11-07 pukul 18 52 13" src="https://user-images.githubusercontent.com/62195104/200303695-9d3cd981-5a6f-4c66-94b6-3429751f283c.png">


## 2. Penulisan

_Markdown_ juga memungkinkan kita untuk menuliskan kata dalam berbagai format tulisan. Berikut adalah beberapa contoh format tulisan dan cara penulisannya:

1. **Huruf Tebal**

  ```markdown
  **Huruf Tebal**
  ```
2. _Huruf Miring_

  ```markdown
  _Huruf Miring_ atau *Huruf Miring*
  ```

3. `Monospace`

  ```markdown
  `Monospace`
  ```

4. ~~Dicoret~~

  ```markdown
  ~~Dicoret~~
  ```

5. [Tautan](https://learn.himpasikom.id/)

  ```markdown
  [Tautan](https://learn.himpasikom.id/)
  ```

6. Indentasi

  > Indentasi 1
  
  ```
  > Indentasi 1
  ```

  >> Indentasi 2
  
  ```
  >> Indentasi 2
  ```

7. Garis Horizontal

  ---

  ```
  ---
  ```

## 3. Gambar
Ada pepatah yang mengatakan "satu gambar bisa lebih bernilai dari seribu kata". Dengan adanya gambar / ilustrasi, orang dapat dengan lebih memahami konsep yang ingin disampaikan. Untuk menampilkan gambar di dalam Google Colab caranya hampir sama seperti memasukkan tautan, yang membedakan adalah jika yang ingin ditampilkan berupa gambar maka ditambahkan `!` di depannya. Jika tautan gambar rusak ataupun tidak valid, maka `teks alternatif` yang akan ditampilkan.

```
![teks alternatif](https://i.redd.it/wc9ggkr9t7781.jpg)
```
![teks alternatif](https://i.redd.it/wc9ggkr9t7781.jpg)

## 4. _List_

Dengan _markdown_ kita bisa menuliskan _list_ baik dalam bentuk `berurutan` ataupun `tidak berurutan`. Untuk _list_ berurutan, kita bisa menuliskan ` 1,2,3,4, dan seterusnya `
```
1. Satu
2. Dua
3. Tiga
```
>1. Satu
>2. Dua
>3. Tiga

Adapun untuk _list_ tidak berurutan kita cukup menuliskan simbol * dan hasilnya akan membentuk suatu **_bullet list_**
```
* Satu
* Dua
* Tiga
```
>* Satu
>* Dua
>* Tiga


## 5. _Syntax Highlighting_

Untuk menampilkan tulisan dengan format seperti kode pada _markdown_ , kita bisa menggunakan membungkus tulisan tersebut dengan ` ``` ` (_backticks_).
````markdown
```
a = a + b
```
````

Hasilnya:

```
a = a + b
```

Secara _default_ hasilnya dari sintaks di atas tidak terkait dengan bahasa pemrograman tertentu. Namun jika diinginkan, kita  bisa memberikan format spesifik berdasarkan bahasa pemrograman yang diinginkan, berikut contoh ketika kita ingin menampilkan kode dalam bahasa _python_

````markdown
```python
print('Hello World')
```
````

Hasilnya:

```python
print('Hello World')
```

## 6. Persamaan

Ketika kita menggunakan notebook untuk keperluan penelitian. Kita mungkin perlu untuk menuliskan berbagai macam persamaan dan simbol matematis. Untuk menuliskan persamaan bisa dilakukan dengan menuliskan sintaks $\LaTeX$ dan membungkusnya dengan simbol `$`. Contoh penggunaannya adalah sebagai berikut:

```
$\alpha, \beta, \gamma, \Gamma, \pi, \Pi, \phi, \varphi, \mu, \Phi $
```
$$ \alpha, \beta, \gamma, \Gamma, \pi, \Pi, \phi, \varphi, \mu, \Phi $$

```
$\frac{n!}{k!(n-k)!} = {n \choose k}$
```
$$ \frac{n!}{k!(n-k)!} = {n \choose k} $$

```
$( a ), [ b ], \{ c \}, | d |, \| e \|,\langle f \rangle, \lfloor g \rfloor,\lceil h \rceil, \ulcorner i \urcorner,/ j\backslash$
```
$$( a ), [ b ], \{ c \}, | d |, \| e \|,\langle f \rangle, \lfloor g \rfloor,\lceil h \rceil, \ulcorner i \urcorner,/ j\backslash$$
```
$\sqrt[n]{1+x+x^2+x^3+\dots+x^n}$
```
$$ \sqrt[n]{1+x+x^2+x^3+\dots+x^n} $$

Untuk mempelajari lebih lanjut terkait simbol dan persamaan matematis, kita bisa merujuk ke tautan [berikut ini](https://en.wikibooks.org/wiki/LaTeX/Mathematics).

## 7. Tabel
Terkadang kita ingin menampilkan informasi dalam bentuk tabel. Di dalam _markdown_ kita menggunakan `|` sebagai pemisah antar kolom. Secara _default_, ** _table header_ ** akan ditulis dengan *tebal*, setelah menuliskan baris untuk _header_ kita juga perlu menuliskan baris berisi tanda `-` sebagai pemisah antara ** _table header_ ** dengan konten. Berikut contoh format untuk penulisan tabel:

```markdown
First column name  | Second column name 
-------------------|------------------
Row 1, Col 1       | Row 1, Col 2 
Row 2, Col 1       | Row 2, Col 2 

```

First column name  | Second column name 
-------------------|------------------
Row 1, Col 1       | Row 1, Col 2 
Row 2, Col 1       | Row 2, Col 2 

```
| Nama  | Jabatan      |
|-------|--------------|
| Luffy | Kapten       |
| Zoro  | Wakil Kapten |
```

| Nama  | Jabatan      |
|-------|--------------|
| Luffy | Kapten       |
| Zoro  | Wakil Kapten |

---

Oke kira-kira itulah beberapa hal yang perlu kita ketahui tentang _markdown_ di Google Colab. Untuk teman-teman yang akan ataupun sedang menggunakan Google Colab. Mempelajari _markdown_ bisa menjadi sesuatu yang sangat berguna. Masih banyak hal-hal yang bisa dieksplorasi lebih lanjut terkait dengan _markdown_ diluar dari yang telah disebutkan dalam artikel ini. Demikian, terima kasih dan selamat belajar!

