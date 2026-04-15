
---

[Vissza](../fizika.md)

---

<details>
    <summary>Hőtan</summary>

---

## I. Főtétel: Az energiamegmaradás törvénye
Azt mondja ki, hogy energia nem vész el, csak átalakul. Egy zárt rendszer belső energiájának megváltozása egyenlő a rendszerrel közölt hő és a rendszeren végzett munka összegével.

Képletben: $\Delta U = Q + W$

- $\Delta U$: A belső energia változása.
- $Q$: A rendszerrel közölt hő (ha a rendszer hőt ad le, az értéke negatív).
- $W$: A rendszeren végzett munka (ha a rendszer végez munkát a környezetén, az értéke negatív).

Lényege: Nem létezik elsőfajú perpetuum mobile (olyan gép, amely semmiből állít elő energiát).

## II. Főtétel: Az entrópia és a folyamatok iránya
Míg az első főtétel szerint a jégkocka magától is megfagyhatna a forró teában (ha közben a tea még forróbb lenne), a második főtétel kijelöli a folyamatok valóságos irányát.
- `Megfogalmazás`: A hő magától soha nem megy át hidegebb testről melegebbre, csak fordítva.
- `Entrópia-elven`: Egy izolált rendszer entrópiája (rendezetlensége) spontán folyamatok során csak növekedhet, vagy stagnálhat, de soha nem csökkenhet.

**Lényege**: Nem létezik másodfajú perpetuum mobile (olyan gép, amely a környezetéből elvont hőt veszteség nélkül, 100%-ban munkává alakítaná).

## III. Főtétel: Az abszolút zérus pont elérése (Nernst-tétel)
Ez a tétel a rendszerek viselkedését írja le az abszolút nulla fok ($0 K$, azaz $−273,15 ^\circ C$) közelében.

- `Megfogalmazás`: Véges számú lépésben nem lehet egy test hőmérsékletét abszolút zérusra csökkenteni.
- `Entrópia-elven`: Ahogy a hőmérséklet közelít a $0 K$-hez, a tiszta kristályos anyagok entrópiája is egy határértékhez, a nullához közelít (tökéletes rend).

---

</details>

<details>
    <summary>Örökmozgó fogalma</summary>

---

Az örökmozgó (latinul perpetuum mobile) egy olyan elméleti gép, amely megállás nélkül képes munkát végezni anélkül, hogy külső energiaforrásra lenne szüksége. A fizika törvényei alapján ilyen gép nem létezhet, de a tudománytörténet során két típust is megkülönböztettek aszerint, hogy melyik főtételt sértik meg.

## 1. Elsőfajú örökmozgó
Ez a gép a **termodinamika I. főtétel**ét (az energiamegmaradás törvényét) sértené meg.
- `Fogalma`: Olyan gép, amely több energiát termel, mint amennyit fogyaszt, vagy anélkül végez munkát, hogy energiát venne fel a környezetéből.
- `Miért lehetetlen?` Mert az energia nem keletkezhet a semmiből. Ha egy gép munkát végez ($W$), ahhoz vagy a belső energiájának ($\Delta U$) kell csökkennie, vagy hőt ($Q$) kell felvennie.

## 2. Másodfajú örökmozgó
Ez a típus már trükkösebb, mert az energiamegmaradás törvényét betartaná, viszont a **termodinamika II. főtétel**ét sérti meg.
- `Fogalma`: Olyan gép, amely egyetlen hőtartályból von el hőt, és azt **teljes egészében** (100%-os hatásfokkal) munkává alakítja, anélkül, hogy a környezetében bármilyen más változás történne (például anélkül, hogy hőt adna le egy hidegebb tartálynak).
- `Példa az elgondolásra`: Egy hajó, amely az óceán vizének belső energiáját használná fel a mozgáshoz: lehűtené a tengervizet, és az így nyert energiával hajtaná a propellereket.
- `Miért lehetetlen?` Mert a hő magától csak a melegebb helyről vándorol a hidegebb felé. Ahhoz, hogy munkát nyerjünk, szükség van egy hőmérséklet-különbségre (egy meleg tartályra, ahonnan az energia jön, és egy hidegre, ahová a "felesleg" távozik).

---

</details>
<details>
    <summary>Hőerőgép fogalma</summary>

---

A `hőerőgép` olyan berendezés, amely `hőenergiát alakít át mechanikai munkává`. Működése során egy munkaanyag (például gáz vagy gőz) egy zárt körfolyamatot végez, miközben hőt vesz fel egy magasabb hőmérsékletű forrásból, és a felvett energia egy részét munkára fordítja.

A `termodinamika II. főtétele` miatt a hőerőgépek `soha nem tudják a felvett hőt 100%-ban munkává alakítani`; a maradék energiát "hulladékhő" formájában le kell adniuk egy alacsonyabb hőmérsékletű környezetnek (hőnyelőnek).

### A hőerőgép működési elve
Minden hőerőgép működéséhez három alapvető összetevő szükséges:
- **Meleg tartály (hőforrás)**: Innen veszi fel a gép a $Q_{be}$​ hőenergiát (pl. égéstér, kazán).
- **Munkaanyag**: Ez végzi a tágulást és a munkát (pl. vízgőz, benzin-levegő keverék).
- **Hideg tartály (hőnyelő)**: Ide adja le a gép a fel nem használt $Q_{ki}$​ hőt (pl. hűtővíz, környezeti levegő).

### Csoportosításuk
A hőerőgépeket elsősorban az alapján osztjuk fel, hogy hol történik a hő felszabadítása:
- **Külső égésű gépek**: Az üzemanyag elégetése a gépen kívül történik, a hő egy közvetítő anyagon keresztül jut be.
    - Példa: Gőzgép, gőzturbina, Stirling-motor.
- **Belső égésű gépek**: Az üzemanyag elégetése a munkatérben (pl. hengerben) történik.
    - Példa: Otto-motor (benzinmotor), Diesel-motor, gázturbina, sugárhajtómű.

## Hatásfok ($\eta$ (éta))
A hatásfok megmutatja, hogy a befektetett hő hány százalékából lett hasznos munka. Képlettel:
- $\eta = \frac{W}{Q_{be}} = \frac{Q_{be} - | Q_{ki} |}{Q_{be}}$

Az elméletileg elérhető legnagyobb hatásfokot a Carnot-hatásfok adja meg, amely csak a két hőtartály abszolút hőmérsékletétől ($T$) függ:
- $\eta_{max} = 1 - \frac{T_{hideg}}{T_{meleg}}$

**Fontos**: Ebből látszik, hogy minél nagyobb a hőmérséklet-különbség a forrás és a hűtő között, annál jobb a gép hatásfoka.

---

</details>
<details>
    <summary>Négy halmazállapot fogalma</summary>

---

A fizikában és kémiában a halmazállapot az anyag azon állapota, amelyben bizonyos fizikai tulajdonságai (például az alakja és a térfogata) állandóak vagy meghatározott módon változnak. Bár a mindennapokban hármat látunk leggyakrabban, tudományos szempontból négy alapvető halmazállapotot különböztetünk meg.

## 1. Szilárd halmazállapot
Az anyag részecskéi (atomok, molekulák vagy ionok) szorosan egymás mellett helyezkednek el, és erős vonzóerők tartják őket össze.
- **Alak és térfogat**: Meghatározott alakja és állandó térfogata van.
- **Mozgás**: A részecskék csak rezgőmozgást végeznek a rácspontok körül, nem mozdulnak el egymáshoz képest.
- **Példa**: Jég, vas, kőzet.

## 2. Folyékony halmazállapot
A részecskék közötti vonzóerő elég erős ahhoz, hogy összetartsa őket, de nem elég erős ahhoz, hogy rögzített pozícióban tartsa a részecskéket.
- **Alak és térfogat**: Nincs saját alakja (felveszi az edény alakját), de térfogata állandó és gyakorlatilag összenyomhatatlan.
- **Mozgás**: A részecskék elgördülnek egymáson, szabadon elmozdulhatnak.
- **Példa**: Víz, olaj, higany.

## 3. Légnemű (gáz) halmazállapot
A részecskék közötti vonzóerő elhanyagolható, a részecskék nagy sebességgel mozognak és messze vannak egymástól.
- **Alak és térfogat**: Sem saját alakja, sem saját térfogata nincs; kitölti a rendelkezésre álló teret. Erősen összenyomható.
- **Mozgás**: Rendezetlen, egyenes vonalú, gyors mozgás, gyakori ütközésekkel.
- **Példa**: Levegő, vízgőz, hélium.

## 4. Plazmaállapot
A "negyedik halmazállapot", amely magas hőmérsékleten (vagy erős elektromos tér hatására) jön létre. Ez egy ionizált gáz.
- Fogalma: Olyan gázszerű állapot, amelyben az atomokról az elektronok leszakadtak, így a rendszer szabadon mozgó pozitív ionokból és negatív elektronokból áll.
- Tulajdonság: Mivel töltött részecskékből áll, kiválóan vezeti az elektromosságot és reagál a mágneses mezőre.
- Előfordulása: Ez a leggyakoribb állapot a látható univerzumban (a csillagok anyaga). A Földön természetes módon a villámlásban vagy az északi fényben fordul elő.

## Átmenetek a halmazállapotok között
Az anyag állapotát a hőmérséklet és a nyomás határozza meg. Az átmeneteket az alábbi LaTeX képletekkel/nevekkel jelölhetjük:
- Olvadás: Szilárd $\implies$ Folyékony
- Fagyás: Folyékony $\implies$ Szilárd
- Párolgás / Forrás: Folyékony $\implies$ Gáz
- Lecsapódás: Gáz $\implies$ Folyékony
- Szublimáció: Szilárd $\implies$ Gáz (köztes folyadékfázis nélkül)
- Ionizáció: Gáz $\implies$ Plazma

---

</details>
<details>
    <summary>Boyle-Mariotte törvénye</summary>

---

Az **izoterm** állapotváltozás olyan folyamat, amely során a gáz (vagy más rendszer) **hőmérséklete állandó marad** ($T = állandó$).

Ahhoz, hogy a hőmérséklet ne változzon, a rendszernek folyamatos hőcserében kell állnia a környezetével: ha tágul (és hűlni akarna), hőt kell felvennie; ha összenyomják (és melegedni akarna), hőt kell leadnia.

## 1. Boyle–Mariotte-törvény
Izoterm körülmények között az ideális gáz nyomása ($p$) és térfogata ($V$) fordítottan arányos egymással. Ha a térfogat felére csökken, a nyomás megduplázódik.

**Képletben**: $p \cdot V = állandó$

vagy két állapot összehasonlításakor: $p_{1} \cdot V_{1} = p_{2} \cdot V_{2}$

## 2. Termodinamikai értelmezés (I. főtétel alapján)
Mivel az ideális gáz belső energiája ($\Delta U$) csak a hőmérséklettől függ, izotherm folyamatnál a belső energia változása nulla ($\Delta U = 0$).

Az I. főtétel ($\Delta U = Q + W$) alapján ebből az következik:
$Q = -W$

Ez azt jelenti, hogy az összes közölt hő ($Q$) teljes egészében munkavégzésre ($W$) fordítódik (táguláskor), vagy fordítva: az összenyomáskor befektetett munka hő formájában távozik a rendszerből.

## 3. Grafikus ábrázolás: Az izoterma
A folyamat grafikonja a $p − V$ diagramon egy hiperbola, amelyet izotermának nevezünk.
- Minél magasabb a gáz hőmérséklete, az izoterma annál messzebb helyezkedik el az origótól.
- A görbe alatti terület adja meg a gáz által végzett (vagy rajta végzett) munkát.

## 4. Példa a gyakorlatból
- **Lassú folyamatok**: Ha egy fecskendő végét befogod és nagyon lassan nyomod össze a benne lévő levegőt, a keletkező hőnek van ideje távozni a falon keresztül, így a levegő hőmérséklete nem emelkedik érezhetően.
- **Párolgás**: Amikor a víz forr, a közölt hő nem a hőmérséklet emelésére megy el ($100 ^{\circ} C$ marad), hanem a halmazállapot megváltoztatására (ez is egyfajta izoterm folyamat).

---

</details>

---

[Vissza](../fizika.md)

---
