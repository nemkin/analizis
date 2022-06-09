# Konvergenciakritériumok sorok esetében

## Bármilyen sorok

### Szükséges feltételek

Ha nem teljesül, akkor divergens. (Ha teljesül akkor nem tudjuk.)

- Egy sor csak akkor tud konvergens lenni, ha az elemei $0$-ba tartanak.  
  $\lim\limits_{k\rightarrow{}\infty}a_k = 0$ szükséges, hogy $\sum\limits_{k=0}^{\infty} a_k $ konvergens lehessen.

## Pozitív előjelű sorok

### Szükséges és elégséges feltételek

Ha teljesül, akkor konvergens. Ha nem teljesül, akkor divergens.

- Pozitív előjelű sor esetében a részletösszegek sorozata egyre növekvő lesz. Ha ez a részletösszeg sorozat korlátos, akkor konvergens, ha nem korlátos akkor divergens.
  - Ha van olyan $C$ konstans, hogy $\forall{}n$ $\sum\limits_{k=0}^{n}a_k < C$, akkor konvergens, ha nincs akkor divergens.

### Elégséges feltételek

Itt van ami konvergenciára, van ami divergenciára vonatkozik. Ha teljesül akkor konvergens/divergens. (Ha nem teljesül akkor nem tudjuk.)

- Majoráns / Minoráns kritérium
  - Konvergenciára (Majoráns kritérium): Sor elemei felülről becsülhetők egy konvergens sor elemeivel.  
    Ha $0 < a_n \leq{} c_n$ $\forall{}n$ és $\sum\limits_{n=1}^{\infty}c_n$ konvergens $\Rightarrow$ $\sum\limits_{n=1}^{\infty}a_n$ konvergens.

## Váltakozó előjelű sorok

### Elégséges feltételek

Ha teljesül, akkor konvergens. (Ha nem teljesül akkor nem tudjuk.)

- Leibniz-sor: Váltakozó előjelű sor, aminek az abszolút
  értékeiből képzett sor monoton csökkenő és $0$-ba tart.
  Ez biztosan konvergens.
  - $|a_{n+1}| > |a_n|$ $\forall{}n$ és
    $\lim\limits_{n\rightarrow\infty} |a_n| = 0$
    $\Rightarrow$ $(-1)^n|a_n|$ konvergens, mert Leibniz.
