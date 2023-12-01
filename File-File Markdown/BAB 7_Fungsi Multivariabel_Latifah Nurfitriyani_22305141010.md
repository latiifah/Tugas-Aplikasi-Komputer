# BAB 7_Fungsi Multivariabel_Latifah Nurfitriyani_22305141010
---

# BAB 7 FUNGSI MULTIVARIABEL

Dibuat Oleh :


NAMA  : LATIFAH NURFITRIYANI


KELAS : MATEMATIKA E


NIM   : 22305141010


---



CAKUPAN MATERI MELIPUTI DIANTARANYA :


BAB 7. FUNGSI MULTIVARIABEL


       # Definisi Fungsi Multivariabel


       A. TURUNAN FUNGSI MULTIVARIABEL


          1. TURUNAN FUNGSI ALJABAR


          2. TURUNAN FUNGSI NON ALJABAR (transenden)


             2.1 Turunan Fungsi Trigonometri


             2.2 Turunan Fungsi Eksponensial


             2.3 Turunan Fungsi Logaritma


          3. TURUNAN FUNGSI KOMPOSISI


       B. INTEGRAL FUNGSI MULTIVARIBAEL


          1. INTERGAL FUNGSI ALJABAR


          2. INTERGAL FUNGSI NON ALJABAR


             2.1 Integral Fungsi Trigonometri


             2.2 Integral Fungsi Eksponensial


             2.3 Integral Fungsi Logaritma


          3. INTERGAL FUNGSI KOMPOSISI


       C. APLIKASI FUNGSI MULTIVARIABEL


---

# Definisi


  Fungsi multivariabel adalah fungsi yang memiliki lebih dari satu
variabel bebas. Fungsi multivariabel memetakan setiap kombinasi nilai
dari variabel-variabel bebas ke dalam nilai tunggal dari variabel
terikat.


# Sebelum melakukan perhitungan, fungsi harus didefinisikan di EMT
dengan:


* 
Menggunakan format nama_fungsi := rumus fungsi (untuk fungsi
* numerik),

* 
Menggunakan format nama_fungsi &amp;= rumus fungsi (untuk fungsi
* simbolik, namun dapat dihitung secara numerik),

* 
Menggunakan format nama_fungsi &amp;&amp;= rumus fungsi (untuk fungsi
* simbolik murni, tidak dapat dihitung langsung),

* 
Fungsi sebagai program EMT.


Setiap format harus diawali dengan perintah function (bukan sebagai
ekspresi).


# A. Turunan Fungsi Multivariabel

# 1. Turunan Fungsi Aljabar

 1) Definisi  
    Turunan fungsi aljabar multivariabel adalah turunan yang dihitung  

terhadap satu variabel bebas dari fungsi multivariabel, dengan
mempertahankan variabel bebas lainnya tetap konstan. Turunan fungsi
aljabar multivariabel dapat diekspresikan dalam bentuk umum dengan
menggunakan turunan parsial. Untuk fungsi


$$F(x_1,x_2,...,x_n)$$di mana n adalah jumlah variabel, turunan parsial dapat dinyatakan
sebagai berikut:


$$F' = \frac {\partial {f}} {\partial {x_1}}, \frac {\partial {f}} {\partial {x_2}},..., \frac {\partial {f}} {\partial {x_n}}$$   Pada perhitungan turunan di EMT dapat menggunakan fungsi "diff".  

2) Contoh dan Visualisasi Grafik


\> function F(x,y) &= x^2 + 3\*x\*y - y^2; $F(x,y)


$$-y^2+3\,x\,y+x^2$$\> $showev('diff(F(x,y),x))


$$\frac{d}{d\,x}\,\left(-y^2+3\,x\,y+x^2\right)=3\,y+2\,x$$   Pembuktian:  

$$F(x,y) = x^2 + 3xy - y^2$$$$F_x = 2x + 3y - 0$$$$F_x = 2x + 3y$$\> plot3d("F(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-008.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-008.png)

\> plot3d("2x + 3y",angle=45°): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-009.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-009.png)

\> function F(x,y) &= 3\*x^2\*y + y^3 + x^3\*y; $F(x,y)


$$y^3+x^3\,y+3\,x^2\,y$$\> $showev('diff(F(x,y),y))


$$\frac{d}{d\,y}\,\left(y^3+x^3\,y+3\,x^2\,y\right)=3\,y^2+x^3+3\,x^2$$   Pembuktian:  

$$F(x,y,z) = 3x^2y + y^3 + x^3y$$$$F_y = 3x^2 + 3y^{3-1} + x^3$$$$F_x = 3x^2 + 3y^2+ x^3$$\> plot3d("F(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-015.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-015.png)

\> plot3d("3\*x^2 + 3\*y^2 + x^3"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-016.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-016.png)

\> function F(x,y,z) &= x^4\*z^3 + 4\*y^2 - z^2; $F(x,y,z)


$$x^4\,z^3-z^2+4\,y^2$$\> $showev('diff(F(x,y,z),z))


$$\frac{d}{d\,z}\,\left(x^4\,z^3-z^2+4\,y^2\right)=3\,x^4\,z^2-2\,z$$   Pembuktian:  

$$F(x,y) = x^4z^3 + 4y^2 - z^2$$$$F_z = 3x^4z^{3-1} + 4.0 - 2z^{2-1}$$$$F_z = 3x^4z^2 - 2z$$   # Pada penggambaran grafik menggunakan fungsi implicit  
 Fungsi implisit (implicit function) adalah fungsi yang memuat lebih  

dari satu variabel, berjenis variabel bebas dan variabel terikat yang
berada dalam satu ruas sehingga tidak bisa dipisahkan pada ruas yang
berbeda.


\> plot3d("F(x,y,z)",r=0.5,implicit=1,contourcolor=blue): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-022.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-022.png)

\> plot3d("3\*x^4\*z^2-2\*z",r=0.5,implicit=1,contourcolor=cyan): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-023.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-023.png)

# 2. Turunan Fungsi Non Aljabar

## 2.1 Turunan Fungsi Trigonometri

1) Definisi


   Turunan fungsi trigonometri multivariabel melibatkan penghitungan
turunan parsial fungsi trigonometri yang memiliki lebih dari satu
variabel masukan.


2) Contoh dan Visualisasi Grafik


\> function F(x,y) &= cos(x)\*sin(y); $F(x,y)


$$\cos x\,\sin y$$\> $showev('diff(F(x,y),y))


$$\frac{d}{d\,y}\,\left(\cos x\,\sin y\right)=\cos x\,\cos y$$   Pembutkian:  

$$F(x,y) = cos(x)sin(y)$$$$F_y = cos(x)cos(y)$$\> plot3d("F(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-028.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-028.png)

\> plot3d("cos(x)\*cos(y)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-029.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-029.png)

\> function F(x,y) &= cos(x) - 2\*sin(x)\*cos(y); $F(x,y)


$$\cos x-2\,\sin x\,\cos y$$\> $showev('diff(F(x,y),x))


$$\frac{d}{d\,x}\,\left(\cos x-2\,\sin x\,\cos y\right)=-2\,\cos x\,  \cos y-\sin x$$   Pembuktian:  

$$F(x,y) = cos(x) - 2sin(x)cos(y)$$$$F_x = -sin(x) - 2cos(x)cos(y)$$\> plot3d("F(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-034.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-034.png)

\> plot3d("-sin(x)-2\*cos(x)\*cos(y)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-035.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-035.png)

## 2.2 Turunan Fungsi Eksponensial

1) Definisi


   Turunan fungsi eksponensial multivariabel adalah turunan parsial
dari fungsi yang mengandung fungsi eksponensial dan memiliki lebih
dari satu variabel independen. 


2) Contoh dan Visualisasi Grafik


\> function f(x,y) &= E^(x\*y); $f(x,y)


$$e^{x\,y}$$\> $showev('diff(f(x,y),x))


$$\frac{d}{d\,x}\,e^{x\,y}=y\,e^{x\,y}$$   Pembuktian:  

$$f(x,y) = e^{xy}$$$$[e^{u(x)}]' = e^{u(x)} . u'(x)$$$$f_x = e^{xy} . 1 . y$$$$= ye^{xy}$$\> plot3d("f(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-042.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-042.png)

\> plot3d("y\*E^(x\*y)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-043.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-043.png)

\> function g(x,y) &= E^(x\*y^2+x^2\*y); $g(x,y)


$$e^{x\,y^2+x^2\,y}$$\> $showev('diff(g(x,y),y))


$$\frac{d}{d\,y}\,e^{x\,y^2+x^2\,y}=\left(2\,x\,y+x^2\right)\,e^{x\,y  ^2+x^2\,y}$$   Pembuktian:  

$$g(x,y) = e^{xy^2+x^2y}$$$$g_y = e^{xy^2+x^2y} . x . 2y^{2-1} + x^2 . 1$$$$= (2xy + x^2)e^{xy^2+x^2y}$$\> plot3d("g(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-049.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-049.png)

\> plot3d("(2\*x\*y+x^2)\*E^(x\*y^2+x^2\*y)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-050.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-050.png)

## 2.3 Turunan Fungsi Logaritma

1) Definisi


   Turunan fungsi logaritma multivariabel adalah konsep dalam kalkulus
multivariabel yang berkaitan dengan perhitungan turunan parsial dari
fungsi yang mengandung logaritma alami (logaritma basis e, sering
dilambangkan sebagai ln) dan memiliki lebih dari satu variabel
independen.


2) Contoh dan Visualisasi Grafik


\> function f(x,y) &= ln(x\*y); $f(x,y)


$$\log \left(x\,y\right)$$\> $showev('diff(f(x,y),x))


$$\frac{d}{d\,x}\,\log \left(x\,y\right)=\frac{1}{x}$$   Pembuktian:  

$$f(x,y) = ln(xy)$$$$[ln(u(x))]' = \frac {1} {u(x)} . u'(x)$$$$f_x = \frac {1} {xy} . 1.y$$$$= \frac {1} {x}$$\> plot3d("f(x,y)", angle=90°): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-057.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-057.png)

\> plot3d("1/x", angle = 180°): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-058.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-058.png)

\> function k(x,y) &= ln(x^2+y^2); $k(x,y)


$$\log \left(y^2+x^2\right)$$\> $showev('diff(k(x,y),y))


$$\frac{d}{d\,y}\,\log \left(y^2+x^2\right)=\frac{2\,y}{y^2+x^2}$$   Pembuktian:  

$$k(x,y) = ln(x^2 + y^2)$$$$k_y = \frac {1} {x^2 + y^2} . (0 + 2y^{2-1})$$$$= \frac {1} {x^2 + y^2} . 2y$$$$= \frac {2y} {x^2 + y^2}$$\> plot3d("k(x,y)"): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-065.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-065.png)

\> plot3d("(2\*y)/(x^2+y^2)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-066.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-066.png)

\> function h(x,y,z) &= (ln(x^2+y^2+z^2))/2; $h(x,y,z)


$$\frac{\log \left(z^2+y^2+x^2\right)}{2}$$\> $showev('diff(h(x,y,z),z))


$$\frac{d}{d\,z}\,\left(\frac{\log \left(z^2+y^2+x^2\right)}{2}  \right)=\frac{z}{z^2+y^2+x^2}$$   Pembuktian:  

$$h(x,y,z) = \frac {ln(x^2+y^2+z^2)} {2}$$$$h_z = \frac {1} {2} . \frac {d} {dz} [ln(x^2+y^2+z^2)]$$$$= \frac {\frac {1} {x^2+y^2+z^2} (0+0+2z)} {2}$$$$= \frac {2z} {2(x^2+y^2+z^2)}$$$$= \frac {z} {x^2+y^2+z^2}$$   # Pada penggambaran grafik menggunakan fungsi implicit  
 Fungsi implisit (implicit function) adalah fungsi yang memuat lebih  

dari satu variabel, berjenis variabel bebas dan variabel terikat yang
berada dalam satu ruas sehingga tidak bisa dipisahkan pada ruas yang
berbeda.


\> plot3d("h(x,y,z)",r=1,implicit=2,contourcolor=red): // grafik fungsi


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-074.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-074.png)

\> plot3d("z/(x^2+y^2+z^2)",r=1,implicit=2,contourcolor=orange): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-075.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-075.png)

# 3. Turunan Fungsi Komposisi

1) Definisi


   Turunan fungsi komposisi multivariabel adalah konsep dalam kalkulus
multivariabel yang berkaitan dengan perhitungan turunan dari fungsi
yang merupakan hasil komposisi dari dua atau lebih fungsi.


2) Contoh dan Visualisasi Grafik


\> function g(x,y) &= 2\*x^2 + 3\*y; $g(x,y)


$$3\,y+2\,x^2$$\> function f(x,y) &= x^2 - y; $f(x,y)


$$x^2-y$$\> $showev('diff(g(f(x,y),y),x))


$$\frac{d}{d\,x}\,\left(3\,y+2\,\left(x^2-y\right)^2\right)=8\,x\,  \left(x^2-y\right)$$   Pembuktian:  

$$g'(f(x,y),y) = 2(x^2 - y)^2 + 3y$$$$= 2.2(x^2 - y)(2x - 0) + 0$$$$= 4(2x)(x^2 - y)$$$$= 8x(x^2 - y)$$\> plot3d("g(x,y)"): // grafik fungsi g(x,y)


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-083.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-083.png)

\> plot3d("f(x,y)"): // grafik fungsi f(x,y)


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-084.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-084.png)

\> plot3d("8\*x\*(x^2-y)"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-085.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-085.png)

\> function h(x,y) &= 3\*x + x\*y^2; $h(x,y)


$$x\,y^2+3\,x$$\> function j(x,y) &= 7\*x\*y^3; $j(x,y)


$$7\,x\,y^3$$\> $showev('diff(h(x,j(x,y)),y))


$$\frac{d}{d\,y}\,\left(49\,x^3\,y^6+3\,x\right)=294\,x^3\,y^5$$   Pembuktian:  

$$h'(x,j(x,y)) = 3x + x(7xy^3)^2$$$$h'(x,j(x,y)) = 3x + 49x^3y^6$$$$= 0 + 49x^3(6y^{6-1})$$$$= 294x^3y^5$$\> plot3d("h(x,y)"): // grafik fungsi h(x,y)


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-093.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-093.png)

\> plot3d("j(x,y)"): // grafik fungsi j(x,y)


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-094.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-094.png)

\> plot3d("294\*x^3\*y^5"): // grafik turunan


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-095.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-095.png)

# B. Integral Fungsi Multivariabel

 # Definisi  
   Integral fungsi multivariabel merupakan bentuk operasi matematika  

yang merupakan kebalikan dari operasi turunan dan limit dari jumlah
ataupun suatu luas. Integral lipat merupakan integral tentu dari
fungsi variabel real banyak, seperti f(x, y) atau f(x, y, z).


    # Integral Ganda  

$$\int \int f(x,y) dV$$    # Integral Tiga Kali Lipat  

$$\int \int \int f(x,y,z) dV$$  dV merupakan elemen diferensial yang menunjukkan bahwa Anda  

melakukan integrasi terhadap suatu variabel. Misalkan dx menunjukkan
integral terhadap variabel x, dy menunjukkan integral terhadap
variabel y, dan dz menunjukkan integral terhadap variabel variabel z.


# 1. Integral Fungsi Aljabar

 # Definisi  
   Integral fungsi aljabar multivariabel adalah suatu bentuk integral  

yang didefinisikan oleh fungsi aljabar yang melibatkan dua atau lebih
variabel.


 # Contoh dan Visualisasi Grafik  

1) Integral Tentu


\> function f(x,y) &= 2\*x^2\*y + 3\*x\*y; $f(x,y)


$$2\,x^2\,y+3\,x\,y$$\> $showev('integrate(f(x,y),x,0,2))


$$\int_{0}^{2}{2\,x^2\,y+3\,x\,y\;dx}=\frac{34\,y}{3}$$\> $showev('integrate(('integrate(f(x,y),x,0,2)),y,0,3))


$$\int_{0}^{3}{\int_{0}^{2}{2\,x^2\,y+3\,x\,y\;dx}\;dy}=51$$   Pembuktian:  

     # dx  

$$\int_0^2 (2x^2y + 3xy) dx$$$$= 2y \int_0^2 x^2 dx + 3y \int_0^2 x dx$$$$\int x^n dx = \frac {x^{n+1}} {n+1}$$$$= 2y \left [\frac {x^{2+1}} {2+1} \right]_0^2 + 3y \left [\frac {x^{1+1}} {1+1} \right]_0^2$$$$= \left [\frac {2x^3y} {3} \right]_0^2 + \left [\frac {3x^2y} {2} \right]_0^2$$$$= \frac {16y} {3} + 6y$$$$= \frac {16y + 18y} {3}$$$$= \frac {34y} {3}$$     # dy  

$$\int_0^3 \frac {34y} {3} dy$$$$= \frac {34} {3} \int_0^3 ydy$$$$= \frac {34} {3} \left[\frac {y^2} {2} \right]_0^3$$$$= \frac {34} {3} \times \frac {9} {2}$$$$= 17 \times 3$$$$= 51$$\> plot3d("f(x,y)"): // grafik 


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-115.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-115.png)

\> function k(x,y) &= 4\*y^3 - 2\*x\*y^2; $k(x,y)


$$4\,y^3-2\,x\,y^2$$\> $showev('integrate(k(x,y),y,0,2))


$$\int_{0}^{2}{4\,y^3-2\,x\,y^2\;dy}=\frac{48-16\,x}{3}$$   Pembuktian:  

$$\int_0^2 (4y^3-2xy^2) dy$$$$= 4 \int_0^2 y^3 dy - 2x \int_0^2 y^2 dy$$$$= 4 \frac {y^{3+1}} {3+1}|_0 ^2 - 2x \frac {y^{2+1}} {2+1} |_0^2$$$$= \frac {4y^4} {4} |_0 ^2 - \frac {2xy^3} {3} |_0 ^2$$$$= y^4 |_0 ^2 - \frac {2xy^3} {3} |_0 ^2$$$$= (2^4 - 0^4) - (\frac {2x.2^3} {3} - \frac {2x.0^3} {3})$$$$= 16 - \frac {16x} {3}$$$$= \frac {48 - 16x} {3}$$\> plot3d("k(x,y)",\>contour,color=blue): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-126.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-126.png)

2) Integral Tak Tentu


\> function g(x,y,z) &= 4\*z^3 - 2\*x\*y^2\*z; $g(x,y,z)


$$4\,z^3-2\,x\,y^2\,z$$\> $showev('integrate(g(x,y,z),z))


$$\int {4\,z^3-2\,x\,y^2\,z}{\;dz}=z^4-x\,y^2\,z^2$$\> $showev('integrate(('integrate(g(x,y,z),z)),y))


$$\int {\int {4\,z^3-2\,x\,y^2\,z}{\;dz}}{\;dy}=y\,z^4-\frac{x\,y^3\,  z^2}{3}$$\> $showev('integrate(('integrate(('integrate(g(x,y,z),x)),z)),y))


$$\int {\int {\int {4\,z^3-2\,x\,y^2\,z}{\;dx}}{\;dz}}{\;dy}=x\,y\,z^  4-\frac{x^2\,y^3\,z^2}{6}$$   Pembtuktian:  

 # dz  

$$\int 4z^3 - 2xy^2z dz$$$$= 4 \int z^3 dz - 2xy^2 \int  z dz$$$$= 4 (\frac {z^{3+1}} {3+1}) - 2xy^2 (\frac {z^{1+1}} {1+1})$$$$= z^4 - 2xy^2z^2$$ # dy  

$$\int z^4 - 2xy^2z^2 dy$$$$= z^4 \int 1 dy - 2xz^2 \int y^2 dy$$$$= yz^4 - 2xz^2 \frac {y^{2+1}} {2+1}$$$$= yz^4 - \frac {2xy^3z^2} {3}$$ # dx  

$$\int yz^4 - \frac {2xy^3z^2} {3} dx$$$$= yz^4 \int 1 dx - \frac {2y^3z^2} {3} \int x dx$$$$= xyz^4 - \frac {2y^3z^2} {3} \frac {x^{1+1}} {1+1}$$$$= xyz^4 - \frac {x^2y^3z^2} {3}$$\> plot3d("g(x,y,z)",\>contour,color=red): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-143.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-143.png)

# 2. Integral Fungsi Non Aljabar

## 2.1 Integral Fungsi Trigonometri

 # Definisi  
   Integral fungsi trigonometri multivariabel adalah bentuk integral  

yang melibatkan fungsi trigonometri yang melibatkan dua atau lebih
variabel. Integral ini dapat dihitung dengan menggunakan teknik-teknik
kalkulus seperti integral ganda dan integral tiga kali lipat.


 # Contoh dan Visualisasi Grafik  

1) Integral Tentu


\> function f(x,y) &= cos(x) - sin(y); $f(x,y)


$$\cos x-\sin y$$\> $showev('integrate(f(x,y),y,-1,1))


$$\int_{-1}^{1}{\cos x-\sin y\;dy}=2\,\cos x$$\> $showev('integrate(('integrate(f(x,y),y,-2,2)),y,-1,1))


$$\int_{-1}^{1}{\int_{-2}^{2}{\cos x-\sin y\;dy}\;dy}=8\,\cos x$$   Pembuktian:  

 # Langkah 1  

$$\int_{-1}^1 (cos(x) - sin(y)) dy$$$$= cos(x) \int_{-1}^1 1 dy - \int_{-1}^1 sin(y) dy$$$$= cos(x) y|_{-1}^1 - (- cos(y))|_{-1}^1$$$$= cos(x) (1 - (-1)) + cos(1) - cos(-1)$$$$= cos(x)(2) + 0$$$$= 2cos(x)$$# Langkah 2


$$\int_{-2}^2 2cos(x) dy$$$$= 2cos(x) \int_{-2}^2 1 dy$$$$= 2cos(x) (y)|_{-2}^2$$$$= 2cos(x) (2 - (-2))$$$$= 8cos(x)$$\> plot3d("f(x,y)"): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-158.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-158.png)

2) Integral Tak Tentu


\> function g(x,y) &= cos(4\*x\*y); $g(x,y)


$$\cos \left(4\,x\,y\right)$$\> $showev('integrate(g(x,y),x))


$$\int {\cos \left(4\,x\,y\right)}{\;dx}=\frac{\sin \left(4\,x\,y  \right)}{4\,y}$$   Pembuktian:  

$$\int cos(4xy) dx$$ misalkan u = 4xy maka  

$$\frac {du} {dx} = 4y$$$$dx = \frac {1} {4y} du$$$$= \frac {1} {4y} \int cos(u) du$$$$= \frac {1} {4y} . sin(u)$$$$= \frac {sin(u)} {4y}$$ subtitusi u = 4xy  

$$= \frac {sin(4xy)} {4y}$$\> $showev('integrate(('integrate(g(x,y),x)),x))


$$\int {\int {\cos \left(4\,x\,y\right)}{\;dx}}{\;dx}=-\frac{\cos   \left(4\,x\,y\right)}{16\,y^2}$$   Pembuktian:  

$$\int \frac {sin(4xy)} {4y} dx$$ misalkan u = 4xy maka  

$$\frac {du} {dx} = 4y$$$$dx = \frac {1} {4y} du$$$$= \frac {1} {4y} . \frac {1} {4y} \int sin(u) du$$$$= \frac {1} {16y^2} (-cos(u))$$$$= - \frac {cos(u)} {16y^2}$$ subtitusi u = 4xy  

$$= - \frac {cos(4xy)} {16y^2}$$\> $showev('integrate(('integrate(('integrate(g(x,y),x)),x)),x))


$$\int {\int {\int {\cos \left(4\,x\,y\right)}{\;dx}}{\;dx}}{\;dx}=-  \frac{\sin \left(4\,x\,y\right)}{64\,y^3}$$   Pembuktian:  

$$\int - \frac {cos(4xy)} {16y^2} dx$$ misalkan u = 4xy maka  

$$\frac {du} {dx} = 4y$$$$dx = \frac {1} {4y} du$$$$= - \frac {1} {16y^2} . \frac {1} {4y} \int cos(u) du$$$$= - \frac {1} {64y^3} (sin(u))$$$$= - \frac {sin(u)} {64y^3}$$ subtitusi u = 4xy  

$$= - \frac {sin(4xy)} {64y^3}$$\> plot3d("g(x,y)"): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-184.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-184.png)

## 2.2 Integral Fungsi Eksponensial

 # Definisi  
   Integral dari sebuah fungsi eksponensial multivariabel adalah  

operasi matematika yang menghitung jumlah dari nilai-nilai fungsi
eksponensial tersebut di suatu wilayah dalam beberapa dimensi. 


 # Contoh dan Visualisasi Grafik  

1) Integral Tentu


\> function k(x,y) &= E^(x\*y); $k(x,y)


$$e^{x\,y}$$\> $showev('integrate(k(x,y),x,0,1))


$$\int_{0}^{1}{e^{x\,y}\;dx}=\frac{e^{y}}{y}-\frac{1}{y}$$\> $showev('integrate(('integrate(k(x,y),x,0,2)),x,0,1))


$$\int_{0}^{1}{\int_{0}^{2}{e^{x\,y}\;dx}\;dx}=\frac{e^{2\,y}}{y}-  \frac{1}{y}$$\> plot3d("k(x,y)"): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-188.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-188.png)

2) Integral Tak Tentu


\> function f(x,y) &= E^x - 2\*y; $f(x,y)


$$e^{x}-2\,y$$\> $showev('integrate(f(x,y),x))


$$\int {e^{x}-2\,y}{\;dx}=e^{x}-2\,x\,y$$   Pembuktian:  

$$\int e^x - 2y dx$$$$= \int e^x dx - 2y \int 1 dx$$$$= e^x - 2xy$$\> plot3d("f(x,y)"):


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-194.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-194.png)

## 2.2 Integral Fungsi Logaritma

 # Definisi  
   Integral fungsi logaritma multivariabel adalah bentuk integral yang  

melibatkan fungsi logaritma yang melibatkan dua atau lebih variabel.
Integral ini dapat dihitung dengan menggunakan teknik-teknik kalkulus
seperti integral ganda dan integral tiga kali lipat. 


 # Contoh dan Visualisasi Grafik  

1) Integral Tentu


\> function t(x,y) &= ln(x) + ln(y); $t(x,y)


$$\log y+\log x$$\> $showev('integrate(t(x,y),x,0,1))


$$\int_{0}^{1}{\log y+\log x\;dx}=\log y-1$$   Pembuktian:  

$$\int_0^1 ln(y) + ln(x) dx$$$$= \int ln(x) dx + ln(y) \int 1 dx$$$$= (xln(x) - x) + ln(y)x$$$$= \left [xln(x) + ln(y)x - x \right]_0^1$$$$= (1.ln(1) + ln(y).1 - 1) - (0 + 0 - 0)$$$$= 0 + ln(y) - 1$$$$= ln(y) - 1$$   # Pada penggambaran grafik menggunakan fungsi implicit  
 Fungsi implisit (implicit function) adalah fungsi yang memuat lebih  

dari satu variabel, berjenis variabel bebas dan variabel terikat yang
berada dalam satu ruas sehingga tidak bisa dipisahkan pada ruas yang
berbeda.


\> plot3d("t(x,y)",r=3,implicit=3,contourcolor=red,angle=90°):


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-204.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-204.png)

2) Integral Tak Tentu


\> function g(x,y) &= ln(x+y); $g(x,y)


$$\log \left(y+x\right)$$\> $showev('integrate(g(x,y),y))


$$\int {\log \left(y+x\right)}{\;dy}=\left(y+x\right)\,\log \left(y+x  \right)-y-x$$   Pembuktian:  

$$\int ln(x+y) dy$$   misalkan u = x + y maka  

$$\frac {du} {dy} = 1 \to dy = du$$$$= \int ln(u) du$$$$= uln(u) - u$$   subtitusi u = x + y  

$$= (x + y) ln(x + y) - (x + y)$$$$= (x + y) (ln(x + y) - 1)$$\> plot3d("g(x,y)",r=4,implicit=3,contourcolor=red): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-213.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-213.png)

# 3. Integral Fungsi Komposisi

 # Definisi  
   Integral dari fungsi komposisi multivariabel adalah integral dari  

fungsi yang didefinisikan sebagai hasil komposisi dari dua atau lebih
fungsi dalam beberapa variabel


 # Contoh dan Visualisasi Grafik  

1) Integral Tentu


\> function f(x,y) &= x^2\*y + 2\*x\*y; $f(x,y)


$$x^2\,y+2\,x\,y$$\> function g(x,y) &= y^2 - x\*y; $g(x,y)


$$y^2-x\,y$$\> $showev('integrate(g(f(x,y),y),x,0,1))


$$\int_{0}^{1}{y^2-y\,\left(x^2\,y+2\,x\,y\right)\;dx}=-\frac{y^2}{3}$$   Pembuktian:  

$$\int_0^1 y^2 - y(x^2y+2xy) dx$$$$= \int y^2 - x^2y^2 - 2xy^2 dx$$$$= y^2 \int 1 dx - y^2 \int x^2 dx - 2y^2 \int x dx$$$$= y^2 (x) - y^2 (\frac {x^3} {3}) - 2y^2 (\frac {x^2} {2})$$$$= xy^2 - \frac {x^3y^2} {3} - x^2y^2$$$$= \left[ xy^2 - \frac {x^3y^2} {3} - x^2y^2 \right]_0^1$$$$= (y^2 - \frac {y^3} {3} - y^2) - 0$$$$= - \frac {y^2} {3}$$\> plot3d("g(f(x,y),y)"): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-225.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-225.png)

2) Integral Tak Tentu


\> function h(x,y) &= x\*y - 2; $h(x,y)


$$x\,y-2$$\> function k(x,y) &= x^2 - y^2; $k(x,y)


$$x^2-y^2$$\> $showev('integrate(h(x,k(x,y)),y))


$$\int {x\,\left(x^2-y^2\right)-2}{\;dy}=x\,\left(x^2\,y-\frac{y^3}{3  }\right)-2\,y$$   Pembuktian:  

$$\int x(x^2-y^2) - 2 dy$$$$= \int x^3 - xy^2 - 2 dy$$$$= \int (x^3 - 2) dy - \int xy^2 dy$$$$= (x^3 - 2) \int 1 dy - x \int y^2 dy$$$$= (x^3 - 2)y - \frac {xy^3} {3}$$$$= (x^3y - \frac {xy^3} {3}) - 2y$$$$= x(x^2y - \frac {xy^3} {3}) - 2y$$\> plot3d("h(k(x,y),y)"): // grafik


![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-236.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-236.png)

# C. Aplikasi Fungsi Multivariabel

  # Kurvatur (Kelengkungan Kurva)  

![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-237.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-237.png)

Aslinya, kelengkungan kurva diferensiabel (yakni, kurva mulus yang
tidak lancip) di titik P didefinisikan melalui lingkaran oskulasi
(yaitu, lingkaran yang melalui titik P dan terbaik memperkirakan,
paling banyak menyinggung kurva di sekitar P). Pusat dan radius
kelengkungan kurva di P adalah pusat dan radius lingkaran oskulasi.
Kelengkungan adalah kebalikan dari radius kelengkungan:


$$\kappa =\frac {1}{R}$$dengan R adalah radius kelengkungan. (Setiap lingkaran memiliki
kelengkungan ini pada setiap titiknya, dapat diartikan, setiap
lingkaran berputar 2pi sejauh 2piR.)


Definisi ini sulit dimanipulasi dan dinyatakan ke dalam rumus untuk
kurva umum. Oleh karena itu digunakan definisi lain yang ekivalen.


## Definisi Kurvatur dengan Fungsi Parametrik Panjang Kurva



Setiap kurva diferensiabel dapat dinyatakan dengan persamaan
parametrik terhadap panjang kurva s:


$$\gamma(s) = (x(s),\ y(s)),$$dengan x dan y adalah fungsi riil yang diferensiabel, yang memenuhi:


$$\|\gamma'(s)\|=\sqrt{x'(s)^2+y'(s)^2}=1.$$Ini berarti bahwa vektor singgung


$$\mathbf{T}(s)=(x'(s),\ y'(s))$$memiliki norm 1 dan merupakan vektor singgung satuan.


Apabila kurvanya memiliki turunan kedua, artinya turunan kedua x dan y
ada, maka T'(s) ada. Vektor ini merupakan normal kurva yang arahnya
menuju pusat kurvatur, norm-nya merupakan nilai kurvatur
(kelengkungan):


$$ \begin{aligned}\mathbf{T}(s) &= \mathbf{\gamma}'(s),\\ \mathbf{T}^{2}(s) &=1\ \text{(konstanta)}\Rightarrow \mathbf{T}'(s)\cdot \mathbf{T}(s)=0\\ \kappa(s) &=\|\mathbf {T}'(s)\|= \|\mathbf{\gamma}''(s)\|=\sqrt{x''(s)^{2}+y''(s)^{2}}.\end{aligned}$$Nilai


$$R(s)=\frac{1}{\kappa(s)}$$disebut jari-jari (radius) kelengkungan kurva.


Bilangan riil


$$ k(s) = \pm\kappa(s)$$disebut nilai kelengkungan bertanda.


Untuk kurva yang dinyatakan dengan fungsi implisit


$$F(x,y)=0$$dengan turunan-turunan parsial


$$F_x=\frac{\partial F}{\partial x},\ F_y=\frac{\partial F}{\partial y},\ F_{xy}=\frac{\partial}{\partial y}\left(\frac{\partial F}{\partial x}\right),\ F_{xx}=\frac{\partial}{\partial x}\left(\frac{\partial F}{\partial x}\right),\ F_{yy}=\frac{\partial}{\partial y}\left(\frac{\partial F}{\partial y}\right),$$berlaku


$$F_x dx+ F_y dy = 0\text{ atau } \frac{dy}{dx}=-\frac{F_x}{F_y},$$sehingga kurvaturnya adalah


$$\kappa =\frac {F_y^2F_{xx}-2F_xF_yF_{xy}+F_x^2F_{yy}}{\left(F_x^2+F_y^2\right)^{3/2}}.$$Contoh:


Parabola


$$y=ax^2+bx+c$$dapat dinyatakan ke dalam persamaan implisit


$$ax^2+bx+c-y=0.$$\> function F(x,y) &= a\*x^2+b\*x+c-y; $F(x,y)


$$-y+a\,x^2+b\,x+c$$\> Fx &= diff(F(x,y),x); Fxx &=diff(F(x,y),x,2); Fy &=diff(F(x,y),y); Fxy &=diff(diff(F(x,y),x),y); Fyy &=diff(F(x,y),y,2); $Fx, $Fxx, $Fy, $Fxy, $Fyy


$$0$$![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-253.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-253.png)

![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-254.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-254.png)

![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-255.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-255.png)

![images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-256.png](images/BAB%207_Fungsi%20Multivariabel_Latifah%20Nurfitriyani_22305141010-256.png)

   Pembuktian  

$$\kappa =\frac {F_y^2F_{xx}-2F_xF_yF_{xy}+F_x^2F_{yy}}{\left(F_x^2+F_y^2\right)^{3/2}}.$$$$= \frac {(-1)^2(2a) - 2(2ax+b)(-1)(0) + (2ax+b)^2(0)} {((2ax+b)^2 + (-1)^2)^{\frac {3} {2}}}$$$$= \frac {2a - 0 + 0} {((2ax+b)^2 + 1)^{\frac {3} {2}}}$$$$= \frac {2a} {((2ax+b)^2 + 1)^{\frac {3} {2}}}$$\> function k(x) &= (Fy^2\*Fxx-2\*Fx\*Fy\*Fxy+Fx^2\*Fyy)/(Fx^2+Fy^2)^(3/2); $'k(x)=k(x) // kurvatur parabola tersebut


$$k\left(x\right)=\frac{2\,a}{\left(\left(2\,a\,x+b\right)^2+1\right)  ^{\frac{3}{2}}}$$Hasilnya sama dengan sebelumnya yang menggunakan persamaan parabola
biasa.


