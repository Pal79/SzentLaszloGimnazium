
---

[Vissza](../matematika.md)

---

# Gyökvonás
- $\sqrt(9) = 3$, mert $3^{2} = 9$
- $\sqrt(16) = 4$, mert $4^{2} = 16$
>
Páros gyökvonásnál kikötés kell:
- $[K] a >= 0$ $\rightarrow$ $(\sqrt[n]{a})^{n} = a$
>
Páratlan gyökvonásnál nem kell kikötés:
- $(\sqrt[3]{a})^{3} = a$
### Általános alakja:
$\sqrt[n]{a} = b$, ha $b^{n} = a$
- $a$ = alap (gyök alatti szám)
- $n$ = gyök fokszáma, ha nincs kiírva, akkor $n = 2$
- $b$ = gyökérték

Ha szorzat vagy osztás van a gyök alatt, szétbontható
>
Ez megengedett, mert a gyök szorzásra és osztásra “elosztható”:
>
$\sqrt[n]{a \cdot b} = \sqrt[n]{a} \cdot \sqrt[n]{b}$
>
Példák:
>
$\sqrt[3]{8x^{3}} = \sqrt[3]{8} \cdot \sqrt[3]{x^{3}} = 2x$
>
$\sqrt[4]{16a^{4} \cdot b^{8}} = \sqrt[4]{16} \cdot \sqrt[4]{a^{4}} \cdot \sqrt[4]{b^{8}} = 2ab^{2}$
>
$\sqrt[5]{\frac{32a^{10}}{b^{5}}} = \frac{\sqrt[5]{32a^{10}}}{\sqrt[5]{b^{5}}} = \frac{2a^{2}}{b}$
>
Ha összeadás vagy kivonás van a gyök alatt, nem bontható szét
>
$\sqrt[n]{a + b} \neq \sqrt[n]{a} + \sqrt[n]{b}$
>
$\sqrt[n]{a-b} \neq \sqrt[n]{a} - \sqrt[n]{b}$
>
Példa:
>
$\sqrt{9+16}=\sqrt{25}=5$
>
$\sqrt{9}+\sqrt{16}=3+4=7$
>
Miért nem lehet szétbontani összeadásra?
>
Mert a gyök (és hatványozás) nem lineáris művelet.
>
A gyökvonás nem „tartja meg” az összeadást.
>
Másképp fogalmazva:
>
A gyök nem disztributív az összeadásra.

## Algebrai gyökvonás
$\sqrt[5]{b^{2}}$ másképp írva $(b^{3})^{1/5}$
### Szabály
ha hatványt emelsz hatványra, akkor a kitevőket összeszorod:
>
$(a^{m})^{n} = a^{m \cdot n}$
#### alkalmazás:
$(b^{3})^{1/5} = b^{3 \cdot \frac{1}{5}} = b^{\frac{3}{5}}$
#### tehát:
$\sqrt[5]{b^{3}} = b^{\frac{3}{5}}$
#### Értelmezés:
Az ötödik gyök a $b$ harmadik hatványából ugyanaz, mint $b$ az $3/5$-ödik hatványon. Ezt gyöktelenített formának hívjuk.
## Gyöktelenített alakból vissza gyükvonásos alakba
### Alapösszefüggés:
A két alak ekvivalens (egymásnak megfelel): $\sqrt[n]{a^{m}} = a^{\frac{m}{n}}$, ez visszafelé: $a^{\frac{m}{n}} = \sqrt[n]{a^{m}}$
### Példa:
$b^{\frac{3}{5}}$ visszaalakítva $b^{\frac{3}{5}} = \sqrt[5]{b^{3}}$
>
mivel az $5$ a gyök fokszáma, és a $3$ a gyök alatti hatványkitevő
>
$x^{\frac{7}{2}} = \sqrt[2]{x^{7}} = \sqrt{x^{7}}$
>
$a^{\frac{4}{3}} = \sqrt[3]{a^{4}}$, ez azt jelenti, hogy a harmadik gyök alatt van az $a^{4}$
### Általános szabály:
Ha: $a^{\frac{p}{q}}$, akkor: $a^{\frac{p}{q}} = \sqrt[q]{a^{p}}$
- $p$ - hatványkitevő
- $q$ - gyök fokszáma
## Kiemelés a gyökjel alól
$\sqrt[4]{32}+\sqrt[4]{162} = \sqrt[4]{16 \cdot 2} + \sqrt[4]{81 \cdot 2} = 2\sqrt[4]{2} + 3\sqrt[4]{2} = 5\sqrt[4]{2}$
- Kiinduló kifejezés:
    - $\sqrt[4]{32} + \sqrt[4]{162}$
- gyök alatti számok 'feltörése':
    - A cél, hogy valamilyen egész szám hatványa kerüljön a gyök alá, amit ki tudunk emelni.
        - $32 = 16 \cdot 2$
        - $162 = 81 \cdot 2$
    - tehát:
        - $\sqrt[4]{16 \cdot 2} + \sqrt[4]{81 \cdot 2}$
- szétbontjuk a szorzatokat gyök alatt:
    - szabály:
        - $\sqrt[n]{a \cdot b} = \sqrt[n]{a} \cdot \sqrt[n]{b}$
    - tehát:
        - $\sqrt[4]{16 \cdot 2} = \sqrt[4]{16} \cdot \sqrt[4]{2}$
        - $\sqrt[4]{81 \cdot 2} = \sqrt[4]{81} \cdot \sqrt[4]{2}$
- egyszerűsítsük a gyökökből, amit lehet:
    - tudjuk, hogy:
        - $16 = 2^{4} \rightarrow \sqrt[4]{16} = 2$
        - $81 = 3^{4} \rightarrow \sqrt[4]{81} = 3$
    - tehát:
        - $\sqrt[4]{16} \cdot \sqrt[4]{2} = 2\sqrt[4]{2}$
        - $\sqrt[4]{81} \cdot \sqrt[4]{2} = 3\sqrt[4]{2}$
- helyettesítsük vissza:
    - $\sqrt[4]{32} + \sqrt[4]{162} = 2\sqrt[4]{2} + 3\sqrt[4]{2}$
- azonos gyökös tagok összevonása:
    - mivel mindkét tagban ugyanaz a gyökös rész szerepel ($\sqrt[4]{2}$), ezeket úgy kezeljük, mint az algebrai azonos tagokat (pl: $2x + 3x = 5x$).
    - tehát:
        - $2\sqrt[4]{2} + 3\sqrt[4]{2} = (2 + 3)\sqrt[4]{2} = 5\sqrt[4]{2}$
- így a végső eredmény:
    - $\sqrt[4]{32} + \sqrt[4]{162} = 5\sqrt[4]{2}$
- Ez történt:
    - A gyök alatti számokat felbontottuk hatvány $×$ maradék alakra.
    - A hatványokat kivettük a gyök alól, mert $\sqrt[4]{a^{4}} = a$.
    - A közös gyökös részt ($\sqrt[4]{2}$) tényezőként kezeltük, és az együtthatókat összeadtuk.
# Másodfokú egyenlet három alakja
## Általános alak
Ez egy másodfokú egyenlet, mert a legmagasabb kitevő $x^{2}$
>
$x^{2} - 2x - 3 = 0$
>
$x_{1} = 3$
>
$x_{2} = -1$
>
Ez a kiinduló forma:
>
$a = 1$
>
$b = -2$
>
$c = -3$
- Általános alakban lévő egyenletet a megoldóképlettel tudjuk megoldani: $x_{1,2} = \frac{-b \pm \sqrt{b^{2} - 4ac}}{2a}$
- számok behelyettesítése: $x_{1,2} = \frac{2 \pm \sqrt{(-2)^{2} - 4 \cdot 1 \cdot (-3)}}{2}$
- kiszámoljuk: $x_{1,2} = \frac{2 \pm \sqrt{4 + 12}}{2} = \frac{2 \pm \sqrt{16}}{2} = \frac{2 \pm 4}{2}$
- két megoldás: $x_{1} = 3, x_{2} = -1$
- tehát a gyökök: $3$ és $-1$
## Szorzat alak
Ha már ismerjük a gyököket ($x_{1} = 3, x_{2} = -1$), akkor a másodfokú egyenletet fel tudjuk bontani tényezőkre.
- a szabály: $a(x-x_{1})(x-x_{2}) = 0$
- mivel itt $a = 1$, egyszerűen: $(x-3)(x+1) = 0$
- felbontjuk a zárójeleket: $(x-3)(x+1) = x^{2}+x-3x-3 = x^{2}-2x-3$
- Visszakaptuk az eredeti egyenletet, tehát helyes.
- Ez az alak azt mutatja meg, hogy az egyenlet zérushelyei (vagyis ahol 0 lesz az értéke)
- pontosan azok a számok, ahol valamelyik zárójeles tényező 0 lesz:
    - $x -3 = 0 \rightarrow x = 3$
    - $x + 1 = 0 \rightarrow x = -1$
## Teljes négyzet alak
- Ez az alak a négyzetté egészítés módszeréből születik.
- Cél: a kifejezést úgy írni fel, hogy egy négyzet legyen benne, és valami maradék.
- Kiindulunk az általános alakból: $x^{2}-2x-3=0$
- a trükk: az $x^{2}-2x$ részt "kiegészítjük", hogy tökéletes négyzet legyen
- tudjuk, hogy: $(x-1)^{2} = x^{2}-2x+1$
- ami egyenletünkben viszont csak $(x^{2}-2x)$ szerepel, tehát hiányzik $+1$, amit majd hozzáadunk és kivonunk egyszerre, hogy ne változzon az érték: $x^{2}-2x-3=(x-1)^{2}-1-3$, egyszerűsítve: $(x-1)^{2}-4=0$
- Ez a teljes négyet alak
### Mit is jelent ez?
Ez a forma segít grafikusan értelmezni az egyenletet, mert: $y = (x-1)^{2}-4$ alakban látszik, hogy a parabola csúcspontja ($1,-4$).
### Ellenőrzés
Ha megoldjuk:
- $(x-1)^{2}=4 \rightarrow x-1 = \pm 2$
- $x_{1} = 3$, $x_{2} = -1$
>
Ugyanazokat a gyököket kaptuk, tehát mindhárom alak ugyanazt az egyenletet írja le.
![parabola](../images/parabola.svg)

---

[Vissza](../matematika.md)

---