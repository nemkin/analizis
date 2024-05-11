# Diffegyenletek megoldása

## Szeparálható

$y' - f(x)g(y) = h(x)$

### Szeparálható - Homogén általános megoldása

$y' - f(x)g(y) = 0$

$y' = f(x)g(y)$

1. eset: Van olyan $k$ ahol $g(k) = 0$

- Ilyenkor $y(x) = k$ megoldás, mert:
  - $y'(x) = 0 $
  - $g(y(x)) = g(k) = 0$
  - $0 = f(x)\cdot{}0$

2. eset: $g(k)\neq{}0$

- Ilyenkor oszthatunk vele:
- $\frac{dy}{dx} = f(x)g(y)$
- $\int{}\frac{dy}{g(y)} = \int{}f(x){dx}$

### Szeparálható - Inhomogén partikuláris megoldása

Állandó variálásával

- Kijön valami $y_{H,Á}(x) = k\cdot{}m(x)$.
- Ekkor a partikuláris megoldást $y_{I,P}(x) = k(x)\cdot{}m(x)$ alakban keressük.
- Visszahelyettesítjük ide: $y' - f(x)g(y) = h(x)$.
  - Ez mindig olyan lesz, hogy a $k(x)$ kiesik és a $k'(x)$-et visszaintegráljuk.

## Lineáris n-edrendű

$a_{n-1}y^{(n-1)} + \dots{} + a_2y'' + a_1y' + a_0 y = f(x)$

### Lineáris n-edrendű - Homogén általános megoldása

$a_{n-1}y^{(n-1)} + \dots{} + a_2y'' + a_1y' + a_0 y = 0$

Karakterisztikus egyenlet:

$a_{n-1}\lambda{}^{n-1} + \dots{} + a_2\lambda{}^2 + a_1\lambda{} + a_0 = 0$

Gyökök alapján: Az alábbi felsorolásból kieső $y(x)$-ek összege kell, különböző $k_i$ konstansokkal.

- $\lambda$ egyszeres valós gyök: ($1$ db megoldás lineáris kombinációja)
  - $y_1(x) = k_1\cdot{}e^{\lambda{}x}$
- $\lambda$ $s$-szeres valós gyök: ($k$ db megoldás lineáris kombinációja)
  - $y_1(x) = k_1\cdot{}e^{\lambda{}x}$
  - $y_2(x) = k_2\cdot{}x\cdot{}e^{\lambda{}x}$
  - $\dots{}$
  - $y_1(x) = k_s\cdot{}x^{s-1}\cdot{}e^{\lambda{}x}$
- $\alpha \pm{} \beta{}i$ egyszeres valós gyökpár: ($2$ db megoldás lineáris kombinációja)
  - $y_1(x) = k_1\cdot{}e^{\lambda{}\alpha{}}\cdot{}cos(\beta{}x)$
  - $y_2(x) = k_2\cdot{}e^{\lambda{}\alpha{}}\cdot{}sin(\beta{}x)$
- $\alpha \pm{} \beta{}i$ $s$-szeres valós gyökpár: ($2s$ db megoldás lineáris kombinációja)
  - $y_1(x) = k_1\cdot{}e^{\lambda{}\alpha{}}\cdot{}cos(\beta{}x)$
  - $y_2(x) = k_2\cdot{}e^{\lambda{}\alpha{}}\cdot{}sin(\beta{}x)$
  - $y_3(x) = k_3\cdot{}x\cdot{}e^{\lambda{}\alpha{}}\cdot{}cos(\beta{}x)$
  - $y_4(x) = k_4\cdot{}x\cdot{}e^{\lambda{}\alpha{}}\cdot{}sin(\beta{}x)$
  - $\dots{}$
  - $\dots{}$
  - $y_{2s-1}(x) = k_{2s-1}\cdot{}x^{s-1}\cdot{}e^{\lambda{}\alpha{}}\cdot{}cos(\beta{}x)$
  - $y_{2s}(x) = k_{2s-1}\cdot{}x^{s-1}\cdot{}e^{\lambda{}\alpha{}}\cdot{}sin(\beta{}x)$

### Lineáris n-edrendű - Inhomogén partikuláris megoldása

Kísérletezéssel, ugyanabból a függvényosztályból.

$a_{n-1}y^{(n-1)} + \dots{} + a_2y'' + a_1y' + a_0 y = f(x)$

| $f(x)$ | $y_{I,P}(x)$ |
| - | - |
| $5$ | $A$ |
| $x^3+5x+2$ | $Ax^2+Bx+C$ |
| $cos(x)$ | $Acos(x) + Bsin(x)$ |
| $x^4sin(4x)$ | $(Ax^4+Bx^3+Cx^2+Dx+E)(Fcos(4x)+Gsin(4x))$ |
| $e^{7x}$ | $Ae^{7x}$ |
| $x^2cos(2x)e^{9x}$ | $(Ax^2+Bx+C)(Dcos(2x)+Esin(2x))e^{9x}$ |
