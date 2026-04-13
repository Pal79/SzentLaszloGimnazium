
---

[Vissza](../matematika.md)

---

# Trigonometria
## Derékszögő háromszögnél
> Egy derékszögű háromszög egyik befogójának hossza $5cm$, átfogójának hossza $8cm$.  
> Határozza meg a háromszög másik befogójának hosszát, és a hegyesszögeinek nagyságát.  
![derékszögű háromszög](../images/pitagorasz-001.drawio.svg)  
$b = 5cm$  
$c = 8cm$

Itt használhatjuk a pitagorasz tételt: $a^{2} + b^{2} = c^{2}$

$a^{2} + 5^{2} = 8^{2}$  
$a^{2} + 25 = 64$ $/-25$  
$a^{2} = 39$ $/\sqrt{}$  
$a = 6.24$

Itt a legegyszerűbben a sinus függvényt használom:

$sin\alpha = \frac{a}{c} = \frac{6.24}{8} = 0.78$  
Most számológépen: $shift + sin$  
$\alpha = 51.26^{\circ}$  
Tehát az alfa szög: $51.26^{\circ}$

Végül a legegyszerűbb, kiszámoljuk a $\beta$ szöget:  
$\beta = 180^{\circ} - (90^{\circ} + 51.26^{\circ}) = 38.74^{\circ}$

---

## Általános háromszögnél

> Egy $ABC$ háromszög $AB$ oldalának hossza $9cm$, $BC$ oldalának hossza $8cm$ hosszúságú, az általuk közrezárt szög $72^{\circ}$-os.  
> Határozza meg a háromszög harmadik oldalának hosszát, és a hiányzó szögeinek nagyságát.  
![általános háromszög](../images/pitagorasz-002drawio.svg)

$a = 8cm$  
$c = 9cm$  
$\beta = 72^{\circ}$

$b^{2} = a^{2} + c^{2} - 2ac \cdot cos\beta$  
$b^{2} = 8^{2} + 9^{2} - 2 \cdot 8 \cdot 9 \cdot cos72^{\circ}$  
$b^{2} = 100.5$  $/ \sqrt{}$  
$b = 10.02cm$

$\frac{a}{b} = \frac{sin\alpha}{sin\beta}$  
$\frac{8}{10.02} = \frac{sin\alpha}{sin72^{\circ}}$  
$0.7984 = \frac{sin\alpha}{0.9511}$ $/ \cdot 0.9511$  
$0.7594 = sin\alpha$  
Számológépen: $shift + sin(0.7594)$  
$\alpha = 49.4$

$\gamma = 180^{\circ} - (72^{\circ} + 49.4^{\circ}) = 58.6^{\circ}$