
---

[Vissza](./trigonometria.md)

---

# Derékszögű háromszög – összes trigonometriai alak
## Szinusz összes alakja  
$\sin(\alpha) = \frac{\text{szemközti}}{\text{átfogó}} = \frac{a}{c}$

| Keresett | Képlet |
| :-- | :-- |
| Szemközti befogó (a) | $a = c \cdot sin(\alpha)$ |
| Átfogó (c) | $c = \frac{a}{sin(\alpha)}$ |

## Koszinusz összes alakja  
$\cos(\alpha) = \frac{\text{szomszédos}}{\text{átfogó}} = \frac{b}{c}$

| Keresett | Képlet |
| :-- | :-- |
| Szomszédos befogó (b) | $b = c \cdot cos(\alpha)$ |
| Átfogó (c) | $c = \frac{b}{cos(\alpha)}$ |

## Tangens összes alakja
$\tan(\alpha) = \frac{\text{szemközti}}{\text{szomszédos}} = \frac{a}{b}$

| Keresett | Képlet |
| :-- | :-- |
| Szemközti befogó (a) | $a = b \cdot tan(\alpha)$ |
| Szomszédos befogó (b) | $b = \frac{a}{tan(\alpha)}$ |

## Kotangens összes alakja
$\cot(\alpha) = \frac{\text{szomszédos}}{\text{szemközti}} = \frac{b}{a}$

| Keresett | Képlet |
| :-- | :-- |
| Szomszédos befogó (b) | $b = a \cdot cot(\alpha)$ |
| Szemközti befogó (a) | $a = \frac{b}{cot(\alpha)}$ |

# Tetszőleges háromszög – fő tételek
## Szinusztétel
$\frac{a}{\sin(\alpha)} = \frac{b}{\sin(\beta)} = \frac{c}{\sin(\gamma)}$

| Keresett | Képlet |
| :-- | :-- |
| Oldal (pl.: a) | $a = \frac{sin(\alpha)}{sin(\beta)} \cdot b$ |
| Szög (pl.: $\alpha$) | $\alpha = arcsin (\frac{a \cdot sin(\beta)}{b})$ |

## Koszinusztétel
$c^2 = a^2 + b^2 - 2ab \cdot \cos(\gamma)$

Oldal keresése  
$c = \sqrt{a^2 + b^2 - 2ab \cdot \cos(\gamma)}$

Átrendezve szögre:  
$\cos(\gamma) = \frac{a^2 + b^2 - c^2}{2ab}$

$\gamma = \arccos\left(\frac{a^2 + b^2 - c^2}{2ab}\right)$

| Keresett | Képlet |
| :-- | :-- |
| Oldal (pl.: c) | $c = \sqrt{a^{2} + b^{2} - 2ab \cdot cos(\gamma)}$ |
| Szög (pl.: $\gamma$) | $\gamma = arccos(\frac{a^{2} + b^{2} - c^{2}}{2ab})$ |

## Tangens- és kotangens tétel
### Tangens tétel
$\frac{a - b}{a + b} = \frac{\tan\frac{\alpha - \beta}{2}}{\tan\frac{\alpha + \beta}{2}}$

### Kotangens tétel
$\cot(\gamma) = \frac{a^2 + b^2 - c^2}{4T}$

# Gyors döntési fa – melyik képletet mikor használod?

| Adott | Keresett | Melyik tétel? |
| :-- | :-- | :-- |
| Derékszög + szög + oldal | Másik oldal | sin / cos / tan / cot |
| Derékszög + két oldal | Szög | arctan / arcsin / arccos |
| Két oldal + közbezárt szög | Harmadik oldal | Koszinusztétel |
| Három oldal | Bármelyik szög | Koszinusztétel (szögre rendezvve) |
| Két szög + egy oldal | Másik oldal | Szinusztétel |
| Egy oldal + két szög | Harmadik szög | $180^{\circ} - (\alpha + \beta)$ |
| Két oldal + nem közbezárt szög | Oldal vagy szög | Szinusztétel |

---

[Vissza](./trigonometria.md)

---