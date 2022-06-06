# Komplex számok

## Komplex gyök számítás

Keressük

$ z^n = r \cdot{} (cos(\alpha) + i\cdot{}sin(\alpha)) $  

$n.$ gyökét, amiből $n$ darab van, a $k.$ gyök:

$ z_k = \sqrt[n]{r}\cdot{}(cos(\frac{\alpha{}+2k\pi{}}{n}) + i\cdot{}sin(\frac{\alpha{}+2k\pi{}}{n})) $

# Polinomok

## Másodfokú egyenlet megoldóképlete

$ ax^2 + bx + c = 0  $

$ x_{1,2} = \frac{-b \pm{} \sqrt{b^2 - 4ac}}{2a} $

# Deriválás

$ ln'(|x|) = \frac{1}{x} $

$ ( \frac{f}{g} )' = \frac{f'g - fg'}{g^2} $

# Koordinátarendszerek

[Jakobi-determinánsos számolások](./koordinatarendszerek.md)

## Gömbi koordináták

<img src="./gombi_koordinatak.png" alt="Gömbi koordináták" width=300px>

$ x = r\cdot{}sin(\vartheta)\cdot{}cos(\varphi) $  
$ y = r\cdot{}sin(\vartheta)\cdot{}sin(\varphi) $  
$ z = r\cdot{}cos(\vartheta)$

### Jakobi-determinánsa

$ r^2sin(\vartheta) = $

|   | r |            $\vartheta$            | $\varphi$ |
| - | - | --------------------------------- | --------- |
| x |   |                                   |           |
| y |   | $\frac{\partial{}i}{\partial{}j}$ |           |
| z |   |                                   |           |


## Henger koordináták

<img src="./henger_koordinatak.png" alt="Henger koordináták" width=300px>

$ x = r\cdot{}cos(\varphi)$  
$ y = r\cdot{}sin(\varphi)$  
$ z = z $

### Jakobi-determinánsa

$r = $

|   | r |            $\vartheta$            | $\varphi$ |
| - | - | --------------------------------- | --------- |
| x |   |                                   |           |
| y |   | $\frac{\partial{}i}{\partial{}j}$ |           |
| z |   |                                   |           |

# Trigonometria

$ sin(x+y) = sin(x)cos(y) + cos(x)sin(y) $  
$ sin(x-y) = sin(x)cos(y) - cos(x)sin(y) $  
$ cos(x+y) = cos(x)cos(y) - sin(x)sin(y) $  
$ cos(x-y) = cos(x)cos(y) + sin(x)sin(y) $

$ cos^2(x)+sin^2(x) = 1 $

$ sin(2x) = 2sin(x)cos(x) $  
$ cos(2x) = cos^2(x) - sin^2(x) $

$ cos^2(x) = \frac{1+cos(2x)}{2} $  
$ sin^2(x) = \frac{1-cos(2x)}{2} $

# Fourier-sor

$\Phi(x) = \frac{a_0}{2} + \sum\limits_{k=1}^{\infty} (a_k\cdot{}cos(kx) + b_k\cdot{}sin(kx)) $

$ a_k = \frac{1}{\pi} \int\limits_{0}^{2\pi} f(x)\cdot{}cos(kx)~dx $, ahol $ k=0,1,2,\cdots{} $  
$ b_k = \frac{1}{\pi} \int\limits_{0}^{2\pi} f(x)\cdot{}sin(kx)~dx $, ahol $ k=1,2,\cdots{} $

# Fourier-transzformáció

$ \mathcal{F}(\omega) = \int\limits_{-\infty{}}^{\infty{}}f(x)\cdot{}e^{-i\omega{}x}~dx $

Inverz:

$ f(x) = \frac{1}{2\pi{}}\int\limits_{-\infty{}}^{\infty{}}\mathcal{F}(\omega)\cdot{}e^{i\omega{}x}~d\omega{} $

![./fourier.png](./fourier.png)

# Dirichlet-tétel (5/2)

Feltételek: PIF MOHA

- Periodikus ($2\pi$-n)
- Integrálható ($[0,2\pi]$-n)
- Felbontható ($[0,2\pi]$ véges sok $[\alpha,\beta]$-ra)
  - Monoton ($f(x)$ $[\alpha,\beta]$-n)
  - Határérték a végpontokban létezik és VÉGES ($f(\alpha+0)$ és $f(\beta-0)$ létezik és véges)

Következmények: A Fourier-sora ekkor:

- Pontonként konvergens (mindenhol)
- $ \Phi(x) = \frac{f(x-0)+f(x+0)}{2} $

![./dirichlet.png](./dirichlet.png)
