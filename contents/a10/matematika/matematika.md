
---

## Számhalmazok (A legkisebbtől a legnagyobbig)
A számhalmazokat olyanok mint egymásba ágyazott dobozok. Minden új halmaz bővíti az előzőt.
- $\mathbb{N}$ - **Természetes számok**: A megszámlálásra használt számok.
    - Példa: $0,1,2,105$ (Megjegyzés: a $0$-t Magyarországon általában ideértjük).
- $\mathbb{Z}$ - **Egész számok**: - A természetes számok, azok negatív tükörképei és a nulla.
    - Példa: $−3,−1,0,4$
- $\mathbb{Q}$ - **Racionális számok**: Minden olyan szám, ami felírható két egész szám hányadosaként (törtként). Tizedestört alakban ezek végesek vagy végtelen szakaszosak.
    - Példa: $\frac{3}{4}, -2.5, 0.3 \text{ ami }(\frac{1}{3})$
- $\mathbb{Q^{*}}$ vagy $\mathbb{I}$ - **Irracionális számok**: Azok a számok, amik nem írhatók fel törtként. Végtelen, nem szakaszos tizedestörtek.
    - Példa: $\sqrt{2}, \pi, $
- $\mathbb{R}$ - **Valós számok**: A racionális és irracionális számok együttesen. Minden szám, ami a számegyenesen elhelyezhető.
## Halmazműveletek
Ha van két halmazunk ($A$ és $B$), a következő alapműveleteket végezhetjük velük:
- **Metszet** ($\cap$): A közös elemek. Amik $A$-ban és $B$-ben is benne vannak.
    - Jele: $A \cap B$ ("$A$ metszet $B$")
- **Unió** ($\cup$): Az összes elem. Ami legalább az egyik halmazban benne van (egyesítés).
    - Jele: $A \cup B$ ("$A$ unió $B$")
- **Különbség** ($\setminus$): Azok az elemek, amik az elsőben benne vannak, de a másodikban nem.
    - Jele: $A \setminus B$ ("$A$ mínusz $B$") – vagyis ami $A$-nak sajátja, de $B$-nek nem tagja.
- **Komplementer** ($\overline{A}$): Kiegészítő halmaz. Minden, ami az alaphalmazban (univerzumban) benne van, de az $A$ halmazon kívül esik.
### Példa
- $A=\{1,2,3,4\}$ és $B=\{3,4,5,6\}$.
    - $A \cap B = \{3,4\}$
    - $A \cup B = \{1,2,3,4,5,6\}$
    - $A \setminus B = \{1,2\}$

---

## Műveleti sorrend
### A hivatalos sorrend (PEMDAS / BODMAS szabály)
Zárójelek nélkül a műveleteket az alábbi hierarchia szerint végezzük el balról jobbra haladva:
1. Hatványozás és gyökvonás ($x^{2}, \sqrt{x}$): Ez a legerősebb szint, ha ilyet látsz, ezzel kell kezdeni.
1. Szorzás és osztás ($\cdot,:$): Egyenrangú műveletek. Ha egymás mellett vannak, szigorúan balról jobbra haladva számoljuk őket.
1. Összeadás és kivonás ($+,-$): A leggyengébb szint. Szintén egyenrangúak, balról jobbra haladunk velük.

Klasszikus becsapós feladat: $6 : 2 \cdot 3$
- megoldás balról jobbra haladunk: $6:2=3$, majd $3 \cdot 3 = 9$
### A zárójelek szerepe sima számolásnál
Amit zárójelbe raksz, azt kiemeled a fenti hierarchiából, és kötelező legelőször kiszámolni.  
Ha egymásba ágyazott zárójelek vannak, akkor a szabály: belülről kifelé haladunk.
- Példa az egymásba ágyazott zárójelekre:
    - $2 \cdot [5 + (10 − 3 \cdot 2)]$
        - Legbelső zárójel: $(10 − 3 \cdot 2)$. Ezen belül a szorzás az első: $3 \cdot 2 = 6$.
        - Majd a kivonás: $10 − 6 = 4$.
    - Következő (szögletes) zárójel: $[5 + 4] = 9$.
    - Utolsó lépés (kívül): $2 \cdot 9 = 18$.
## Oszthatóság és Prímszámok
**Oszthatóság**: Egy a egész szám akkor osztója egy b egész számnak, ha az osztás során a maradék nulla.
- Jelölése: $a∣b$ (olvasva: $a \text{ osztja }b$-t). Például: $3∣12$.
- Prímszámok (törzsszámok): Azok a $1$-nél nagyobb természetes számok, amelyeknek pontosan két osztójuk van: az $1$ és önmaguk.
    - Példák: $2,3,5,7,11,13,17,...$ (A $2$ az egyetlen páros prím!)
- Összetett számok: Azok a $1$-nél nagyobb számok, amelyeknek kettőnél több osztójuk van (vagyis felbonthatók prímek szorzatára).
    - A $0$ és az $1$: Speciális számok, sem nem prímek, sem nem összetettek.

A **számelmélet** alaptétele: Minden 1-nél nagyobb összetett szám egyértelműen (a tényezők sorrendjétől eltekintve) felbontható prímszámok szorzatára. Ezt hívjuk **prímtényezős felbontás**nak.
## Legnagyobb közös osztó: lnko(a,b) vagy gcd(a,b)
A két vagy több szám közös osztói közül a legnagyobb.
- Kiszámítása (Prímtényezős módszer):
    1. Bontsuk fel a számokat prímek szorzatára.
    1. Keressük meg a közös prímtényezőket.
    1. Vegyük őket az előforduló legkisebb hatványon, majd szorozzuk össze őket.
    - Példa: lnko($24,36$)
        - $24 = 2^{3} \cdot 3^{1}$
        - $36 = 2^{2} \cdot 3^{2}$
        - Közös prímek a legkisebb hatványon: $2^{2} és 3^{1}$.
        - $\text{lnko}( 24, 36 ) = 2^{2} \cdot 3^{1} = 4 \cdot 3 = 12$.
## Legkisebb közös többszörös: lkkt[a,b] vagy lcm(a,b)
A két vagy több számnak az a legkisebb pozitív többszöröse, amelyet mindegyik szám maradék nélkül oszt. (Például törtek közös nevezőre hozásakor használjuk).
- Kiszámítása:
    1. Bontsuk fel a számokat prímek szorzatára.
    1. Vegyük az összes előforduló prímtényezőt (a nem közösekkel együtt).
    1. Mindegyiket az előforduló legnagyobb hatványra emeljük, majd összeszorozzuk őket.
    - Példa: $\text{lkkt}[24,36]$
        - $24 = 2^{3} \cdot 3^{1}$
        - $36 = 2^{2} \cdot 3^{2}$
        - Az összes prím a legnagyobb hatványon: $2^{3} \text{ és } 3^{2}$.
        - $\text{lkkt}[24,36] = 2^{3} \cdot 3^{2} = 8 \cdot 9 = 72$.
## A két fogalom kapcsolata
Bármely két pozitív egész számra igaz, hogy a számok szorzata egyenlő az $lnko$-juk és $lkkt$-jük szorzatával:
- $a \cdot b = \text{lnko}(a,b) \cdot \text{lkkt}[a,b]$

---

## Alapfogalmak: Pont, Egyenes, Félegyenes, Szakasz
A geometriában a pontot és az egyisenest nem definiáljuk, ezek úgynevezett alapfogalmak.
- **Pont**: Kiterjedés nélküli hely a térben. (Jele: nagybetű, pl. $A,B$)
- **Egyenes**: Mindkét irányban végtelen, egydimenziós vonal. (Jele: kisbetű, pl. $e,f$)
- **Félegyenes**: Egy pontból kiinduló, egy irányban végtelen egyenes darab.
- **Szakasz**: Egy egyenes két pontja (végpontok) közé eső része. Van mérhető hossza. (Jele: $AB$)
## Szögfajták
A szögeket a nagyságuk (fok) alapján csoportosítjuk $0^{\circ} \text{ és } 360^{\circ}$ között:
- Nullszög: $0^{\circ}$
- Hegvesszög: $0^{\circ} < \alpha < 90^{\circ}$
- Derékszög: $\alpha = 90^{\circ}$ (jelölése a rajzokon egy kis ív ponttal, vagy négyzet)
- Tompaszög: $90^{\circ} < \alpha < 180^{\circ}$
- Egyenesszög: $\alpha = 180^{\circ}$ (egy egyenest alkot a két szára)
- Homorúszög: $180^{\circ} < \alpha < 360^{\circ}$
- Teljes szög: $\alpha = 360^{\circ}$
## Háromszögek tulajdonságai
A háromszögeket két szempont szerint szoktuk csoportosítani: oldalaik vagy szögeik szerint.
### Csoportosítás oldalak szerint:
- **Általános**: Minden oldala különböző hosszúságú.
- **Egyenlő szárú**: Két oldala (szárak) egyenlő. Az alaphoz tartozó szögei is egyenlők.
- **Egyenlő oldalú (szabályos)**: Minden oldala és minden belső szöge egyenlő ($60^{\circ}$-osak).
### Csoportosítás szögek szerint:
- **Hegyesszögű**: Minden szöge hegyesszög ($< 90^{\circ}$).
- **Derékszögű**: Van egy $90^{\circ}$-os szöge. Oldalaira igaz a Pitagorasz-tétel ($a^{2} + b^{2} = c^{2}$).
- **Tompaszögű**: Van egy tompaszöge ($>90^{\circ}$).
### Aranyszabályok háromszögekre:
- **Belső szögek összege**: Mindig $180^{\circ}$ ($\alpha + \beta + \gamma = 180^{\circ}$).
- **Háromszög-egyenlőtlenség**: Bármely két oldal összegének nagyobbnak kell lennie a harmadik oldalnál ($a + b > c$).
## Négyszögek tulajdonságai
A négyszögeket leggyakrabban a párhuzamos oldalaik száma alapján rendszerezzük:
- **Trapéz**: Olyan négyszög, amelynek van legalább egy pár párhuzamos oldala.
- **Paralelogramma**: Olyan trapéz, amelynek két pár párhuzamos oldala van. (Szemközti oldalai és szögei egyenlők, átlói felezik egymást).
- **Rombusz**: Olyan paralelogramma, amelynek minden oldala egyenlő. (Átlói merőlegesek egymásra és felezik a belső szögeket).
- **Téglalap**: Olyan paralelogramma, amelynek minden szöge derékszög. (Átlói egyenlő hosszúak).
- **Négyzet (A "tökéletes" négyszög)**: Egyszerre rombusz és téglalap. Minden oldala egyenlő és minden szöge $90^{\circ}$.
- **Deltoid**: Olyan négyszög, amely két-két egymás melletti egyenlő oldalú háromszögből állítható össze (szimmetrikus az egyik átlójára, átlói merőlegesek).

**Aranyszabály négyszögekre**: A belső szögek összege minden esetben $360^{\circ}$.

---

## Pitagorasz tétel
Kizárólag derékszögű háromszögekre érvényes, és összeköti a háromszög oldalainak hosszát.
### Mik azok a befogók és mi az az átfogó?
A derékszögű háromszög oldalait a derékszöghöz ($90^{\circ}$-os szöghöz) való viszonyuk alapján nevezzük el:
- **Befogók ($a \text{ és } b$)**: Az a két oldal, amelyek közrefogják a derékszöget (innen a név: "befogják" a szöget). Ezek egymásra merőlegesek.
- **Átfogó ($c$)**: A derékszöggel szemközti oldal. Ez mindig a háromszög leghosszabb oldala (mivel a legnagyobb szöggel szemben a leghosszabb oldal áll).

**A tétel kimondva**:
- Derékszögű háromszögben a két befogó hosszának négyzetösszege egyenlő az átfogó hosszának négyzetével.
- Matematikai képlettel leírva: $a^{2} + b^{2} = c^{2}$
### Hogyan fejezzük ki az ismeretlent?
A feladatokban általában két oldal hossza adott, és a harmadikat kell kiszámolnod. Attól függően, hogy mi hiányzik, a képletet át kell alakítanunk gyökvonással.
#### Ha az ÁTFOGÓ ($c$) az ismeretlen:
Ez a legegyszerűbb eset. Csak gyököt vonsz az eredeti képlet mindkét oldalából: $c = \sqrt{a^{2} + b^{2}}$
- Példa:
    - $a = 3$
    - $b = 4$
    - $c = \sqrt{3^{2} + 4^{2}} = \sqrt{9 + 16} = \sqrt{25} = 5$
#### Ha az egyik BEFOGÓ (a vagy b) az ismeretlen:
Ilyenkor az eredeti képletből először ki kell vonni a másik befogó négyzetét, hogy az ismeretlen magára maradjon, majd utána jön a gyökvonás. (A lényeg: a leghosszabb oldal négyzetéből vonjuk ki az ismert rövid oldal négyzetét).
1. Ha $a$-t keressük: $a^{2} = c^{2} - b^{2} \implies a = \sqrt{c^{2} - b^{2}}$
1. Ha $b$-t keressük: $b^{2} = c^{2} - a^{2} \implies b = \sqrt{c^{2} - a^{2}}$
- Példa:
    - $c = 10$
    - $a = 6$
    - $b = \sqrt{10^{2} - 6^{2}} = \sqrt{100 - 36} = \sqrt{64} = 8$

---

## Terület- és kerületszámítás: Síkidomok formulái.
A kerület ($K$) a síkidomot határoló vonalak teljes hossza (vagyis ha körbesétálnád a formát), míg a terület ($T$) a síkidom által lefedett kétdimenziós felület nagysága.
### Háromszög
A háromszög területéhez az egyik oldalra és a hozzá tartozó magasságra (az oldalra merőleges, szemközti csúcsból induló egyenesre) van szükség.
- **Kerület**: A három oldal összege.
    - $K = a + b + c$
- **Terület**: Oldal szorozva a hozzá tartozó magassággal, osztva kettővel.
    - $T = \frac{a \cdot m_{a}}{2} = \frac{b \cdot m_{b}}{2} = \frac{c \cdot m_{c}}{2}$
### Négyzet és Téglalap
A leginkább magától értetődő síkidomok, ahol a szögek mind derékszögek.
- **Négyzet** (minden oldala $a$)
    - **Kerület**: $K = 4 \cdot a$
    - **Terület**: $T = a^{2}$ (vagyis $a \cdot a$)
- **Téglalap** ($a$ és $b$ oldalak)
    - **Kerület**: $K = 2 \cdot (a + b)$ vagy $K = 2a + 2b$
    - **Terület**: $T = a \cdot b$
### Paralelogramma és Rombusz
Olyan négyszögek, amelyeknek a szemközti oldalaik párhuzamosak, de a szögeik nem feltétlenül derékszögek (kissé "el vannak dőlve").
- **Paralelogramma** ($a$ és $b$ oldalak)
    - **Kerület**: $K = 2 \cdot (a + b)$ pont, mint a téglalapnál
    - **Terület** Oldal szorozva a hozzá tartozó magassággal: $T = a \cdot m_{a} = b \cdot m_{b}$
### Rombusz (minden oldala $a$)
Mivel minden oldala egyenlő, a kerülete a négyzetével egyezik meg, a területe pedig kiszámolható az átlói ($e$ és $f$) segítségével is, mert azok merőlegesek egymásra.
- **Kerület**: $K = 4 \cdot a$
- **Terület**: $T = a \cdot m_{a}$ vagy $T = \frac{e \cdot f}{2}$
### Trapéz
Olyan négyszög, amelynek van két párhuzamos oldala (ezeket alapoknak hívjuk: $a$ és $c$), valamint két szára ($b$ és $d$).
- **Kerület**: A négy oldal összege.
    - $K = a + b + c + d$
- **Terület**: A két párhuzamos oldal átlaga megszorozva a magassággal.
    - $T = \frac{a + c}{2} \cdot m$
### Kör
A körnél bejön a képbe a $\pi$ (pí) állandó, melynek értéke kerekítve $3,14$. A számításokhoz a kör sugarát ($r$) vagy az átmérőjét ($d = 2 \cdot r$) használjuk.
- **Kerület** (a körvonal hossza):
    - $K = 2 \cdot r \cdot \pi$
- **Terület**:
    - $T = r^{2} \cdot \pi$

---

## Sokszögek: Külső és belső szögek összege, és a konvex sokszögek átlóinak száma.
### Belső szögek összege ($S_{n}$)
Ahogy egy sokszög oldalszáma növekszik, úgy nő a belső szögeinek összege is. A trükk az, hogy bármelyik konvex sokszöget fel lehet osztani háromszögekre úgy, hogy egyetlen csúcsból meghúzzuk az összes lehetséges átlót.
Mivel minden háromszög belső szögeinek összege $180^{\circ}$, a képlet a következő: $S_{n} = (n - 2) \cdot 180^{\circ}$
- Nézzük meg a gyakorlatban:
    - Háromszög ($n=3$): $(3 - 2) \cdot 180^{\circ} = 1 \cdot 180^{\circ} = 180^{\circ}$
    - Négyszög ($n=4$): $(4 − 2) \cdot 180^{\circ} = 2 \cdot 180^{\circ} = 360^{\circ}$
    - Ötszög ($n=5$): $(5 − 2) \cdot 180^{\circ} = 3 \cdot 180^{\circ} = 540^{\circ}$
#### Szabályos sokszögek:
Ha a sokszög szabályos (minden oldala és szöge egyenlő), akkor az egy darab belső szög nagyságát úgy kapod meg, hogy az összeget elosztod a csúcsok számával: $\frac{(n-2) \cdot 180^{\circ}}{n}$
### Külső szögek összege
A külső szögek a belső szögek melletti kiegészítő szögek (egy egyenesre esnek velük, így egy belső és a mellette lévő külső szög összege mindig $180^{\circ}$).  
Itt van a matematika egyik legszebb meglepetése: bármilyen konvex sokszög külső szögeinek összege mindig pontosan $360^{\circ}$, függetlenül attól, hogy hány oldala van!
- $S_{kulso} = 360^{\circ}$

Mindegy, hogy egy háromszögről vagy egy $100$ oldalú sokszögről beszélünk, ha körbehaladva összeadjuk a külső szögeket, pontosan egy teljes kört kapunk.
### Konvex sokszögek átlóinak száma ($d_{n}$)
Az átló olyan szakasz, ami két nem szomszédos csúcsot köt össze. Ha szeretnénk kiszámolni, hány átlója van összesen egy $n$ oldalú sokszögnek, a logikát kell követnünk:
1. Egy csúcsból nem húzhatunk átlót önmagába, és a két közvetlen szomszédjába sem (mert azok az oldalak). Tehát egy csúcsból $n−3$ darab átló indul.
1. Mivel $n$ darab csúcsunk van, ezt megszorozzuk $n$-el: $n \cdot (n − 3)$.
1. Ezzel viszont minden átlót pontosan kétszer számoltunk meg (egyszer az egyik végéről, egyszer a másikról), így az eredményt el kell osztanunk kettővel.
- A képlet tehát: $d_{n} = \frac{n \cdot (n - 3)}{2}$

- Példa:
    - Háromszög $(n = 3)$: $\frac{3 \cdot (3 - 3)}{2} = \frac{0}{2} = 0$ - A háromszögnek nincs átlója.
    - Négyszög $(n = 4)$: $\frac{4 \cdot (4 - 3)}{2} = \frac{4 \cdot 1}{2} = 2$ - a négyszögnek két átlója van.
    - Hatszög $(n = 6)$: $\frac{6 \cdot (6 - 3)}{2} = \frac{6 \cdot 3}{2} = \frac{18}{2} = 9$

---

## Algebra és Egyenletek
### Betűs kifejezések alapjai
A betűs kifejezésekben a betűk (változók) tetszőleges számokat jelölnek.
- **Tagok és együtthatók**: A $3x^{2}$ kifejezésben a $3$-as szám az együttható (megmutatja, hányszor vesszük a betűs részt), az $x$ a változó, a $2$-es pedig a kitevő.
- **Egynemű kifejezések**: Azok a tagok, amelyekben a betűs rész és azok kitevői teljesen megegyeznek. Csak az egynemű kifejezéseket lehet összevonni (összeadni/kivonni).
    - Összevonható (egynemű): $5x + 3x = 8x$ vagy $4ab^{2} − 2ab^{2} = 2ab^{2}$
    - NEM vonható össze: $2x + 3y$ vagy $5x + 5x^{2}$ (a kitevő eltér!)
### Nevezetes azonosságok
A nevezetes azonosságok olyan sűrűn előforduló zárójeles szorzások, amelyek végeredményét érdemes fejből tudni, mert rengeteg időt spórolnak meg az egyenletek megoldása vagy a kiemelések során.
#### Két tag összegének négyzete
Amikor egy összeget önmagával szorzunk meg: $(a + b)(a + b)$.
- $(a + b)^{2} = a^{2} + 2ab + b^{2}$
- Szabály: Az első tag négyzete, meg az első és második tag szorzatának a kétszerese, meg a második tag négyzete.
- Példa: $(x + 3)^{2} = x^{2} + 2 \cdot x \cdot 3 + 3^{2} = x^{2} + 6x + 9$
#### Két tag különbségének négyzete
Ugyanaz, mint az előző, de a két tag között kivonás van: $(a − b)(a − b)$.
- $(a − b)^{2} = a^{2} − 2ab + b^{2}$
- Figyelem: A $2ab$ előtti jel változik mínuszra, a $b^{2}$ előtti jel marad pozitív (mivel negatív szám négyzete is pozitív)
- Példa: $(2x − 5)^{2} =(2x)^{2} − 2 \cdot 2x \cdot 5 + 5^{2} = 4x^{2} − 20x + 25$
#### Két tag összegének és különbségének szorzata
Ez a "kedvenc", mert a középső tagok kiesnek a beszorzás után, így egy nagyon tiszta eredményt kapunk.
- $(a + b)(a − b) = a^{2} − b^{2}$
- Szabály: Az első tag négyzete mínusz a második tag négyzete. (Négyzetek különbsége).
- Példa: $(x + 4)(x − 4) = x^{2} − 4^{2} = x^{2} − 16$
### Gyakori hiba
A legtipikusabb hiba, amit diákok elkövetnek: $(a + b)^{2} \neq a^{2} + b^{2}$

Ha elfelejted a középső tagot ($2ab$), az olyan, mintha egy ház építésénél kihagynád a tartófalakat. Mindig gondolj a fenti szabályokra!

---

## Elsőfokú egyenletek és egyenlőtlenségek
### Elsőfokú egyenletek megoldása lépésről lépésre
Az egyenletek megoldásánál az ekvivalens (egyenértékű) átalakítások szabályait követjük: amit teszünk az egyenlet bal oldalával, pontosan ugyanazt kell tennünk a jobb oldalával is.
- A megoldás menetének aranyat érő lépései:
    - **Zárójelek felbontása**: Ha van zárójel, beszorzással szabaduljunk meg tőle.
    - **Közös nevező (ha tört van)**: Szorozzuk be az egyenletet a nevezők legkisebb közös többszörösével.
    - **Összevonás**: Mindkét oldalon külön-külön vonjuk össze az egynemű kifejezéseket (az x-eket az x-ekkel, a számokat a számokkal).
    - **Rendezés (Mérlegelv)**: Vigyük az összes x-es tagot az egyik oldalra, a sima számokat a másik oldalra (ellentétes művelettel!).
    - **Osztás az együtthatóval**: Osszuk el mindkét oldalt az x előtt álló számmal.
    - **Ellenőrzés**: Behelyettesítéssel nézzük meg, igaz-e az egyenlőség.

#### Példa:
Keressük meg $x$ értékét
- $3(x − 2) + 5 = 2x + 7$
1. Zárójel felbontása: $3x - 6 + 5 = 2x + 7$ 
1. Összevonás bal oldalon: $3x − 1 = 2x + 7$
1. Rendezés:
    - Vonjunk ki mindkét oldalból $2x$-et, hogy az $x$-ek balra kerüljenek:
        - $3x − 2x − 1 = 7 \implies x − 1 = 7$
    - Most adjunk mindkét oldalhoz 1-et, hogy a szám jobbra kerüljön:
        - $x = 7 + 1 \implies x = 8$
### Elsőfokú egyenlőtlenségek
Az egyenlőtlenségekben egyenlőségjel ($=$) helyett relációs jeleket használunk: $<$ (kisebb), $>$ (nagyobb), $\le$ (kisebb vagy egyenlő), $\ge$ (nagyobb vagy egyenlő).

A lépések $99\%$-ban megegyeznek az egyenletekével, de van egy rendkívül fontos szabály, amin a legtöbb pont elúszik a dolgozatokban:
- AZ ARANYSZABÁLY: Ha az egyenlőtlenség mindkét oldalát negatív számmal szorozzuk vagy osztjuk, a relációs jel megfordul! (A $<$ jelből $>$ lesz, és fordítva).
#### Miért fordul meg a jel?
Tudjuk, hogy $2 < 5$. Ha mindkét oldalt megszorozzuk $−1$-el, a számok $−2$ és $−5$ lesznek. A számegyenesen a $−2$ van közelebb a nullához, tehát az a nagyobb. Így a jelnek meg kell fordulnia, hogy igaz legyen az állítás: $−2 > −5$.
#### Példa:
- $−3x + 4 < 10$
- Vonjunk ki mindkét oldalból $4$-et:
    - $−3x < 6$
- Most osszuk el mindkét oldalt $−3$-al (mivel negatívval osztunk, megfordul a jel!):
    - $x > \frac{-3}{6}$
    - $x > −2$

Ennek a megoldásnak a végeredménye nem egyetlen szám, hanem egy egész számhalmaz: minden olyan szám, ami nagyobb, mint $−2$.

$$
\begin{aligned}
3x - 1 &= 2x + 7 \quad / -2x \\
x - 1 &= 7 \quad / +1 \\
x &= 8
\end{aligned}
$$

---

## Szöveges feladatok felírása
### A fordítási szótár (Hogyan lesz a szóból matematikai jel?)
A magyar szövegekben bizonyos kulcsszavak mindig ugyanazt a matematikai műveletet rejtik. Ha ezeket felismered, nyert ügyed van:

| Magyar szövegfordulat | Matematikai művelet | Példa |
| :-: | :-: | :-: |
| valamennyivel több / nagyobb | $+$ (összeadás) | A $5$-tel nagyobb, mint $B$: $\implies A=B+5$ |
| valamennyivel kevesebb / kisebb |	$−$ (kivonás) | A $3$-mal kisebb, mint $B$: $\implies A=B−3$ |
| valahányszorosa / - szorosa | $\cdot$ (szorzás) | $A$ a $B$ $4$-szerese: $\implies A=4⋅B$ |
| valahányad része / - ad része | $:$ vagy tört (osztás) | $A$ a $B$ harmadrésze: $\implies A=\frac{3}{B}$ |
| ugyanannyi / megegyezik | $=$ (egyenlőségjel) | $A$ ugyanannyi, mint $B$: $\implies A=B$ |

### A 4 lépéses stratégia
1. lépés: Válaszd ki az ismeretlent ($x$)!
    - A legjobb döntés általában az a dolog, amiről a legkevesebb információt tudjuk a szövegből, vagy amire a kérdés rákérdez.
1. lépés: Írd fel a többi adatot az $x$ segítségével!
    - Ne vezess be feleslegesen $y,z,w$ betűket, ha nem muszáj. Próbálj meg mindent az $x$-hez viszonyítani a fenti szótár alapján.
1. lépés: Keresd meg az összefüggést (Az egyenletet)!
    - A szövegben mindig van egy mondat, ami az egyensúlyt teremti meg (pl. "ha összeadjuk őket...", "ekkor ugyanannyi lesz..."). Ez alapján állítsd fel a mérleget (az egyenletet).
1. lépés: Megoldás és ellenőrzés a szöveg alapján!
    - Oldd meg az egyenletet, de a kapott eredményt ne az egyenletbe, hanem a szövegbe helyettesítsd vissza, hogy lásd, van-e értelme (például egy ember életkora nem lehet $−5$ év, vagy a zsebpénz összege nem lehet fél forint).
### Három klasszikus feladattípus sémája
#### Életkoros feladatok (Az időutazás)
- **Szöveg**: Apa most $3$-szor idősebb, mint a fia. $5$ év múlva az apuka már csak $2,5$-szer lesz idősebb. Hány évesek most?
    - Készíts egy kis táblázatot a MÚLT / JELEN / JÖVŐ oszlopokkal, és ne felejtsd el, hogy az idő mindenkire ugyanúgy telik! (Ha elmúlik $5$ év, mindenkinek az életkorához hozzá kell adni $5$-öt).

| Szereplő | Jelenlegi kor | Kor $5$ év múlva |
| :-: | :-: | :-: |
| Fiú | $x$ | $x+5$ |
| Apa | $3x$ | $3x+5$ |

- Az egyenlet: $5$ év múlva az apa kora ($3x+5$) egyenlő lesz a fiú korának ($x+5$) a $2,5$-szeresével:
    - $3x + 5 = 2,5 \cdot (x + 5)$
#### Számjegyes feladatok (A helyiértékek)
- **Szöveg**: Egy kétjegyű számban a tizesek száma $2$-vel nagyobb az egyesekénél...
    - Ha egy kétjegyű szám jegyei $a$ és $b$, akkor a szám valódi értéke nem $a \cdot b$, hanem $10a+b$ (hiszen az a a tizes helyiértéken áll).
        - Példa: A $73$ az valójában $10 \cdot 7 + 3$.
        - Ha a számjegyeit felcseréljük, az új szám értéke: $10b+a$ lesz.
#### Keverési feladatok (Töménység, oldatok)
- **Szöveg**: Összeöntünk $2$ liter $10\%$-os és $3$ liter $20\%$-os sóoldatot. Hány százalékos lesz a keverék?
    - A trükk: Az egyenletet mindig a tiszta anyagra (a sóra, a savra, az alkoholra) írjuk fel. A tiszta anyag tömege nem változik az összeöntés során: I. oldat sója, $+$ II. oldat sója $=$ Keverék sója.
    - Képlettel: $2 \cdot 0.10 + 3 \cdot 0.20 = (2 + 3) \cdot x$

---

## Másodfokú egyenletek
### A másodfokú egyenlet kanonikus (általános) alakja
- Mielőtt bármit számolnál, az egyenletet mindig úgy kell átrendezned, hogy a jobb oldalon nulla álljon. Ez a kiindulópont: $ax^{2} + bx + c = 0$
- Ahol a betűk ($a,b,c$) valamilyen ismert számok (együtthatók), és nagyon fontos a szerepük:
    - **a**: Az $x^{2}$ előtti szám (ez sosem lehet $0$, különben az egyenlet nem lenne másodfokú).
    - **b**: Az $x$ előtti szám.
    - **c**: A konstans (sima szám), ami mögött nincs $x$.
- **Példa**:
    - Ha az egyenleted $2x^{2} −5x + 3 = 0$, akkor a számaid:
        - $a=2$,
        - $b=(−5)$,
        - $c=3$.
### A másodfokú egyenlet megoldóképlete
Ha megvannak az $a,b,c$ értékei, nincs más dolgod, mint behelyettesíteni őket ebbe a formulába:

$$
\begin{aligned}
x_{1,2} = \frac{-b \pm \sqrt{b^{2} - 4 \cdot a \cdot c}}{2 \cdot a}
\end{aligned}
$$

A $\pm$ (plusz-mínusz) jel azt jelenti, hogy a másodfokú egyenletnek legfeljebb két megoldása lehet ($x_{1}$ és $x_{2}$). Az egyiknél a gyök előtt hozzáadsz, a másiknál kivonsz.
#### Példa:
Oldjuk meg a $x^{2} −5x + 6 = 0$ egyenletet!
##### Adatok:
- $a = 1$ (mivel nincs kiírva semmi az $x^{2}$ előtt)
- $b = (-5)$
- $c = 6$
##### Behelyettesítés:
$$
\begin{aligned}
x_{1,2} = \frac{-(-5) \pm \sqrt{(-5)^{2} - 4 \cdot 1 \cdot 6}}{2 \cdot 1} \\
x_{1,2} = \frac{5 \pm \sqrt{25 - 24}}{2} \\
x_{1,2} = \frac{5 \pm \sqrt{1}}{2} \implies \frac{5 \pm 1}{2} \\
\\
x_{1} = \frac{5 + 1}{2} = \frac{6}{2} = 3 \\
x_{2} = \frac{5 - 1}{2} = \frac{4}{2} = 2
\end{aligned}
$$
### A diszkrimináns (D) – *Hány megoldás van?*
A megoldóképletben a gyök alatt lévő kifejezést ($b^{2} − 4ac$) diszkriminánsnak nevezzük, és $D$-vel jelöljük. Ez a szám határozza meg, hogy egyáltalán hány valós megoldása lesz az egyenletnek:
- Ha $D > 0$ (pozitív): A gyök alatt pozitív szám van, így $2$ különböző valós megoldás lesz (mint a fenti példánkban).
- Ha $D = 0$: A gyök alatt nulla van, $\sqrt{0} = 0$. Mivel a plusz nulla és a mínusz nulla ugyanaz, $1$ darab valós megoldás lesz (ezt kétszeres vagy gyöknek is nevezzük).
- Ha $D < 0$ (negatív): Mivel a valós számok körében negatív számból nem tudunk négyzetgyököt vonni, az egyenletnek nincs valós megoldása.
### Hiányos másodfokú egyenletek
Ha a $b$ vagy a $c$ értéke nulla, nem kötelező a hosszú megoldóképletet használni, sokkal gyorsabban is célba érhetsz:
- Ha $c = 0$ (pl. $x^{2} − 4x = 0$)
    - **Megoldás**: Emelj ki $x$-et:
        - $x(x-4) = 0$
    - Egy szorzat csak akkor lehet nulla, ha valamelyik tényezője nulla. Így a két megoldás azonnal látszik:
        - $x_{1} = 0$
        - $x - 4 = 0 \implies x_{2} = 4$
- Ha $b = 0$ (pl. $x^{2} − 9 = 0$)
    - **Megoldás**: Rendezd át és vonj gyököt!
        - $x^{2} = 9 \implies x = \pm \sqrt{9} \implies x_{1} = 3, x_{2} = (−3)$

---

## Függvények és Hatványok
### Hatványozás és azonosságai
A hatványozás egy azonos tényezőkből álló szorzás rövidítése. A $a^{n} kifejezésben az $a$ az alap (amit szorzunk), az $n$ pedig a kitevő (hányszor szorozzuk meg az alapot önmagával).
#### A legfontosabb hatványazonosságok:
Ha ezeket ismered, bármilyen összetett algebrai törtet vagy kifejezést le tudsz egyszerűsíteni:
- **Azonos alapú hatványok szorzása**: Az alap változatlan marad, a kitevőket összeadjuk.
    - $a^{n} \cdot a^{m} = a^{n+m}$
- **Azonos alapú hatványok osztása**: Az alap változatlan marad, a kitevőket kivonjuk egymásból.
    - $\frac{a^{n}}{a^{m}} = a^{n - m}$
- Hatvány hatványozása: Az alapot a kitevők szorzatára emeljük.
    - $(a^{n})^{m} = a^{n \cdot m}$
- Szorzat és tört hatványozása: Tagoltan, minden tényezőt külön-külön hatványozunk.
    - $(a \cdot b)^{n} = a^{n} \cdot a^{m}$
    - $(\frac{a}{b})^{n} = \frac{a^{n}}{b^{n}}$
#### Két speciális eset:
1. A nulla kitevő ($a^{0}$): Bármely nullától különböző szám a nulladik hatványon mindig $1$.
    - Pl.: $5^{0} = 1$.
1. A negatív kitevő ($a^{-n}$): A negatív kitevő nem negatív számot jelent, hanem a szám reciprokát (törtbe fordulást). $a^{-n} = \frac{1}{a^{n}}$
    - Pl.: $2^{-3} = \frac{1}{2^{3}} = \frac{1}{8}$
## Függvények alapjai
A függvény egy egyértelmű hozzárendelés: az $X$ halmaz (értelmezési tartomány) minden egyes eleméhez hozzárendeljük az $Y$ halmaz (képhalmaz) pontosan egy elemét.
- **Értelmezési tartomány** ($É.T.$ vagy $Df$): Azok a számok, amiket behelyettesíthetsz a függvénybe ($x$ értékek). Figyelem: nullával nem oszthatunk, és páros gyök alatt nem állhat negatív szám!
- Értékkészlet ($É.K.$ vagy $Rf$): Azok a számok, amiket eredményül kaphatunk ($y$ értékek).
## Alapvető függvénytípusok és grafikonjaik
A függvényeket a koordináta-rendszerben ($X$ és $Y$ tengely) ábrázoljuk. Íme a 4 leggyakoribb alapfüggvény:
1. Lineáris függvény (Elsőfokú)
    - **Képlete**: $f(x) = ax + b$
    - **Grafikonja**: Egy egyenes. Az $a$ határozza meg a meredekséget (ha pozitív, emelkedik; ha negatív, lejt), a $b$ pedig azt a pontot, ahol az egyenes metszi az $Y$ tengelyt.
1. Másodfokú függvény
    - **Képlete**: $f(x) = x^{2}$
    - **Grafikonja**: Egy parabola ($U$ alakú görbe). Ha az $x^{2}$ előtt negatív jel van ($−x^{2}$), a parabola lefelé nyitott
1. Abszolútérték-függvény
    - **Képlete**: $f(x) = ∣x∣$
    - **Grafikonja**: Egy $V$ alakú törésvonal. Mindent, ami negatív lenne, a pozitív tartományba tükröz (mivel a távolság nem lehet negatív).
1. Négyzetgyökfüggvény
    - **Képlete**: $f(x) = \sqrt{x}$
    - **Grafikonja**: Egy fél fekvő parabola. Csak a pozitív térfelen létezik ($x \ge 0$), mert negatív számból nem vonhatunk valós gyököt.

---

## Statisztika, Valószínűség és Logika
### Statisztika (Adatok elemzése)
A statisztika feladata az adatok gyűjtése, rendszerezése és jellemzése. Két fő fogalomcsoportot kell itt ismerni:
1. Mutatók, amelyek a halmaz "közepét" keresik:
    - **Átlag** (Számtani közép): Az adatok összege elosztva az adatok számával.
        - $\bar{x} = \frac{x_{1} + x_{2} + ... + x_{n}}{n}$
    - **Medián**: A nagyság szerint sorba rendezett adatok közül a pontosan középen lévő érték.
        - Ha az adatok száma páratlan: a középső szám. (Pl. $1,3,7,8,10 \implies \text{ medián } = 7$)
        - Ha az adatok száma páros: a két középső szám átlaga. (Pl. $1,3,7,9 \implies \frac{3 + 7}{2} = 5$)
    - **Módusz**: A leggyakrabban előforduló elem (a "legnépszerűbb" adat). egy adathalmaznak lehet több módusza is.
1. Mutatók, amelyek a halmaz "szóródását" (szétterülését) mérik:
    - Terjedelem: A legnagyobb és a legkisebb adat különbsége ($x_{max} - x_{min}$).
    - **Szórás** ($\sigma$): Megmutatja, hogy az adatok átlagosan milyen messze esnek a számtani középtől (az átlagtól). Ha a szórás kicsi, az adatok sűrűn az átlag körül vannak; ha nagy, akkor nagyon szétszórtak.
### Valószínűségszámítás
A valószínűségszámítás azt méri meg, hogy mekkora eséllyel következik be egy esemény egy véletlen kísérlet során.
#### A klasszikus valószínűség képlete:
Valamiért ezt a képletet szoktuk a legtöbbet használni. Egy $A$ esemény valószínűsége $P(A)$:

$P(A) = \frac{\text{Kedvező esetek száma}}{Összes esetek száma}$

##### Példa: Kockadobásnál mi a valószínűsége, hogy páros számot dobunk?
- **Összes eset**: $1,2,3,4,5,6 \implies (6 \text{darab})$
- **Kedvező esetek**: $2,4,6 \implies (3 \text{darab})$
- $P(\text{páros} = \frac{3}{6} = \frac{1}{2} = 0.5$
    - $0.5 \cdot 100 = 50\%$
#### Fontos szabályok:
- A valószínűség értéke mindig $0$ és $1$ között van (vagyis $0\%$ és $100\%$ között).
- **Lehetetlen esemény**: $P=0$ (pl. $7$-est dobni egy normál kockával).
- **Biztos esemény**: $P=1$ (pl. $7$-nél kisebbet dobni).
- **Egymást kizáró események**: Ha két esemény nem történhet meg egyszerre, a valószínűségeik összeadódnak ($P(A \text{ vagy } B)=P(A)+P(B)$).
### Logika (Igaz és Hamis állítások)
A matematikai logikában kijelentésekkel dolgozunk, amelyekről egyértelműen eldönthető, hogy $\text{Igaz } (I / 1) \text{ vagy } \text{Hamis } (H / 0)$. Ezeket a kijelentéseket logikai műveletekkel kötjük össze.
#### Legyen két állításunk: $A$ és $B$.

| Művelet neve | Jelölése | Hétköznapi megfelelője | Mikor IGAZ? |
| :-: | :-: | :-: | :-: |
| Negáció (Tagadás) | $\neg A$ vagy $A^{-}$ | Nem $A$ | Ha az eredeti állítás hamis volt. |
| Konjunkció | $A \wedge B$ | $A$ és $B$ | Csak akkor, ha mindkettő igaz egyszerre. |
| Diszjunkció | $A \vee B$ | A vagy B | Ha legalább az egyik igaz (megengedő vagy). |
| Implikáció | $A \implies B$ | Ha $A$, akkor $B$ | Mindig igaz, kivéve ha az igazból ($A$) hamis ($B$) következik. |

---

## Geometria II. és Trigonometria
### Hasonlóság és középpontos hasonlóság
Két síkidom hasonló, ha alakjuk megegyezik, de a méretük eltérhet. (Gondolj egy fotó kicsinyítésére vagy nagyítására).
- **A hasonlóság feltétele**: * A megfelelő szögeik egyenlők.
    - A megfelelő oldalaik aránya állandó ($k$). Ezt a $k$ számot hasonlósági aránynak nevezzük.
- **Területek és térfogatok aránya**: Ha az oldalak $k$-szorosára változnak:
    - A terület $k^{2}$-szeresére változik ($T^{'} =k^{2} \cdot T$).
    - A térfogat $k^{3}$-szorosára változik ($V^{'} = k^{3} \cdot V$).
### Derékszögű háromszögek trigonometriája (Szögfüggvények)
A szögfüggvények valójában oldalarányokat jelentenek a derékszögű háromszögben. Egy kiválasztott $\alpha$ hegyesszöghöz képest az oldalakat így nevezzük:
- **Átfogó ($c$)**: A derékszöggel szemközti, leghosszabb oldal.
- **Szöggel szemközti befogó ($a$)**: Az $\alpha$ szöggel szemben lévő oldal.
- **Szög melletti befogó ($b$)**: Az $\alpha$ szög mellett fekvő oldal.
#### A 4 alapvető szögfüggvény:
1. $sin \alpha = \frac{\text{szöggel szemközti befogó}}{\text{átfogó}} = \frac{a}{c}$
1. $cos \alpha = \frac{\text{szög melletti befogó}}{\text{átfogó}} = \frac{b}{c}$
1. $tan \alpha = \frac{\text{szöggel szemközti befogó}}{\text{szög melletti befogó}} = \frac{a}{b}$
1. $cot \alpha = \frac{\text{szög melletti befogó}}{\text{szöggel szemközti befogó}} = \frac{b}{a}$
##### Hogyan jegyezd meg?
A szinusz mindig a szemközti oldallal kezdődik (sz-sz), a koszinusz pedig a mellette lévővel. A tangens és kotangens pedig csak a két befogó aránya.
### Általános háromszögek trigonometriája (Szinusz- és Koszinusztétel)
Ha a háromszög nem derékszögű, a fenti egyszerű arányok nem működnek. Ilyenkor a következő két nehéztüzérségi tételhez kell nyúlnunk:
#### Szinusztétel
Bármely háromszögben két oldal hosszának aránya megegyezik a szemközti szögek szinuszainak arányával.

$$
\begin{aligned}
\frac{a}{b} = \frac{sin \alpha}{sin \beta} \text{ vagy másként }
\frac{a}{sin \alpha} = \frac{b}{sin \beta} = \frac{c}{sin \gamma}
\end{aligned}
$$

##### Mikor használjuk?
Ha ismerünk a háromszögben egy teljes "párt" (egy oldalt és a szemközti szöget), plusz még egy hiányzó adatot.
### Koszinusztétel
Olyan, mint a Pitagorasz-tétel felturbózott változata, ami minden háromszögre igaz.

$$
\begin{aligned}
c^{2} = a^{2} + b^{2} - 2ab \cdot cos \gamma
\end{aligned}
$$

##### Mikor használjuk?
1. Ha ismerünk két oldalt és a köztük lévő szöget, és a harmadik oldalt keressük.
1. Ha ismerjük mind a három oldalt, és egy szöget akarunk kiszámolni.
### Trigonometrikus területképlet
Ha egy háromszögnek ismerjük két oldalát ($a$ és $b$) és a köztük lévő szöget ($\gamma$), akkor a magasság kiszámolása nélkül is megkaphatjuk a területet:

$$
\begin{aligned}
T = \frac{a \cdot b \cdot sin \gamma}{2}
\end{aligned}
$$

---

## Térgeometria
### Testek felszíne és térfogata
A képletek megértéséhez jegyezz meg két alapvető jelölést:
- $T_{alap}$: az alaplap területe (ez a test formájától függően lehet kör, négyzet, téglalap stb.)
- $T_{palást}$: a test oldallapjainak (az "oldalfalának") az összterülete.
#### Téglatest (a,b,c oldalélű)
Olyan test, mint egy gyufásdoboz, melynek minden lapja téglalap.
- **Felszín**: 3 pár különböző téglalapból áll, mindegyikből kettő van.

$$
\begin{aligned}
A = 2 \cdot (a \cdot b + a \cdot c + b \cdot c)
\end{aligned}
$$

- **Térfogat**: Alapterület szorozva a magassággal.

$$
\begin{aligned}
V = a \cdot b \cdot c
\end{aligned}
$$

#### Egyenes henger ($r$ sugarú, $m$ magasságú)
Képzelj el egy konzervdobozt. Az alapja és a fedőlapja is egy $r$ sugarú kör, a kiterített palástja pedig egy téglalap.
- **Alapterület**: $T_{alap} = r^{2} \cdot \pi$
- **Palástterület**: $T_{palást} = 2 \cdot r \cdot \pi \cdot m$
- **Felszín**: Két alaplap plusz a palást.
    - $A = 2 \cdot T_{alap} + T_{palást} = 2 \cdot r^{2} \cdot \pi + 2 \cdot r \cdot \pi \cdot m$
- **Térfogat**: Alapterület szorozva a magassággal.
    - $V = r^{2} \cdot \pi \cdot m$
#### Egyenes kúp ($r$ alap-sugarú, $m$ testmagasságú, $s$ alkotójú)
Képzelj el egy fagylalttölcsért vagy egy boszorkánykalapot. Az $s$ (alkotó) a kúp csúcsát és az alap körvonalát összekötő ferde szakasz.
- **Felszín**: Alaplap (kör) plusz a palást (ami egy körcikk).
    - $A = r^{2} \cdot \pi + r \cdot \pi \cdot s$
- **Térfogat**: Mivel a kúp csúcsos test, a térfogata pontosan a harmadrésze egy ugyanilyen alapú és magasságú hengernek!
    - $V = \frac{r^{2} \cdot \pi \cdot m}{3}$
##### Pitagorasz-kapcsolat a kúpban:
A kúp sugara ($r$), testmagassága ($m$) és alkotója ($s$) egy derékszögű háromszöget zár be, így mindig igaz rájuk, hogy: $r^{2} + m^{2} = s^{2}$
#### Gúla ($T_{alap}$ alapterületű, $m$ magasságú)
Olyan csúcsos test, mint az egyiptomi piramisok. Az alaplapja bármilyen sokszög lehet (szabályos gúlánál általában négyzet vagy háromszög), a palástját pedig háromszögek alkotják.
- **Felszín**: Az alapterület és a palástot alkotó háromszögek területeinek összege.
    - $A = T_{alap} + T_{palást}$
- **Térfogat**: Mivel ez is csúcsos test, a térfogat itt is harmadolandó!
    - $V = \frac{T_{alap} \cdot m}{3}$

---

## Százalékszámítás
### A három alapfogalom
1. **Alap ($A$)**: Az a teljes mennyiség, aminek a százalékát keressük. Ez felel meg a $100\%$-nak. (A „valaminek” a... kifejezésben a „valami”).
1. **Százalékláb ($p$)**: A százalékban megadott szám, vagyis hogy a századrészekből mennyit veszünk. (Jele mögött mindig ott a $\%$).
1. **Százalékérték ($É$)**: Az alapnak a megadott százaléka konkrét számban (mennyiségben) kifejezve.
### A 3 alapeset és kiszámításuk
A képletek helyett a legegyszerűbb, ha a százaléklábat fejben azonnal átváltod tizedestörtté (elosztod $100$-al), és azzal dolgozol.
#### A százalékérték ($É$) kiszámítása
##### Mikor használjuk?
Ha megvan a teljes összeg, és tudni akarod, mennyi annak a valahány százaléka.
- **A szabály**: Az alapot megduzzasztod/megszorzod a százalék tizedestört alakjával.
    - $É = A \cdot \frac{p}{100}$
- **Példa**: Mennyi a $400$ gramm $15\%$-a?
    - Váltsd át a $15\%$-ot: $15:100=0.15$
    - Szorozz: $400 \cdot 0.15 = 60 \text{gramm}$
#### A százalékláb (p) kiszámítása
##### Mikor használjuk?
Ha tudod a rész és az egész mennyiségét is, és az a kérdés, hogy ez hány százalékot jelent.
- **A szabály**: A részt (értéket) elosztod az egésszel (alappal), majd az eredményt megszorzod $100$-al, hogy százalékot kapj.
    - $p = \frac{É}{A} \cdot 100$
- **Példa**: Egy $30$ fős osztályból $6$-an jelesek matekból. Hány százalék ez?
    - Oszd el a részt az egésszel: $\frac{6}{30} = 0.2$
    - Váltsd át százalékká: $0.2 \cdot 100 = 20\%$
#### Az alap ($A$) kiszámítása
##### Mikor használjuk?
Ha csak egy részletet ismersz, és azt, hogy ez a részlet hány százaléka az egésznek. A cél a $100\%$ megtalálása.
- **A szabály**: A százalékértéket elosztod a százalékláb tizedestört alakjával.
    - $A = \frac{É}{\frac{p}{100}}$
- **Példa**: Egy kabát ára $20\%$-os leértékelés után (vagyis a kabát az eredeti ár $20\%$-a) $8000 Ft$. Mennyi volt az eredeti ár?
    - Váltsd át a $20\%$-ot: $0.2$
    - Oszd el az értéket a törttel: $8000 : 0.2 = 40000 Ft$
#### Gyors és praktikus mindennapi trükkök
A boltban vagy számlák fizetésekor nem kell füzetért nyúlni, ezekkel a mentális rövidítésekkel azonnal kapsz eredményt:
- **$10\%$ kiszámítása**: Csak told el a tizedesvesszőt egy hellyel balra (oszd el $10$-el). (Pl. $4500 Ft$ $10\%$-a $= 450 Ft$).
- **$1\%$ kiszámítása**: Told el a vesszőt két hellyel balra (oszd el $100$-al). (Pl. $4500 Ft$ $1\%$-a $= 45 Ft$).
- **$5\%$ kiszámítása**: Keresd meg a $10\%$-ot, és felezd meg.
- **$25\%$ kiszámítása**: Negyedeld el az összeget (oszd el $4$-gyel).
- **$50\%$ kiszámítása**: Felezd meg az összeget (oszd el $2$-vel).

---
