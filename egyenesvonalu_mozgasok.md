# Egyenesvonalú mozgások

> Forrás: a könyv II. fejezete (2.1–2.11 + Összefoglalás, Kérdések, Feladatok).
> Ez a modul az egész mechanika alapja: itt tanuljuk meg a hely, sebesség és gyorsulás pontos jelentését.

---

## 1. Téma bevezetése

### Mi a téma?
Egy **anyagi pont (részecske)** mozgásának leírása **egyenes vonal mentén**, azaz egy dimenzióban. Ezt a területet **kinematikának** nevezzük.

### Mi a téma jelentése?
- A kinematika két kérdésre válaszol: **hol?** és **mikor?** Vagyis megmondja, hol van a test az idő függvényében, és hogyan változik a helye.
- **Nem** azzal foglalkozik, *miért* mozog (az erők a későbbi modulok témái), csak azzal, *hogyan*.
- A pont geometriai fogalom, a valódi tárgyak (autó, labda) nem pontok. A kiterjedt test mozgása viszont leírható így:
  - a **tömegközéppont** mozgásával,
  - plusz a test tömegközéppont körüli forgásával.
- Ezért elég egyetlen pont mozgásával kezdeni. A *részecske* szót tágan használjuk: lehet teniszlabda, a Föld vagy akár egy galaxis is. Ha csak a tömegközéppont elmozdulása érdekel (a forgásokat, rezgéseket elhanyagoljuk), a test mindig egyetlen részecskének tekinthető.

### Mindennapi előfordulás, felhasználás
- **Mindennapokban:** autó gyorsítása és fékezése, lift, metró, futó, leejtett tárgy, felfelé dobott labda.
- **Fizikában:**
  - a mechanika minden további fejezetének alapja (síkbeli mozgás, erők, energia),
  - szabadesés és hajítások (állandó gyorsulású mozgás),
  - csillagászat (galaxisok távolodása, Hubble-törvény), geológia (kontinentális lemezek mozgása).
- A mozgásfajták közül a legérdekesebbek azok, amelyeknél a sebesség **változik**.

---

## 2. Téma kifejtése

### 2.1 Alapfogalmak

#### Tér és idő (Newton szerint)
- **Homogén tér:** a tér tulajdonságai nem függnek a helytől.
- **Izotrop tér:** a tér tulajdonságai nem függnek az iránytól.
- **Abszolút idő:** egyenletesen telik, nem gyorsítható és nem lassítható.
- A tér és az idő Newton szerint egymástól független.
- **Fontos megjegyzés:** a pontosabb kísérletek szerint ez a kép csak közelítés (nagy sebességeknél, galaxisközi vagy atomi méreteknél másként viselkedik a világ). Ezekkel a későbbi fejezetek foglalkoznak. Itt a Newton-féle tér- és időfogalmat használjuk.

#### Koordinátarendszer és vonatkoztatási rendszer
- **Koordinátarendszer:** a pont helyének megadására szolgál. Kell hozzá egy **origó**, **irányított tengely(ek)** és **skála** (egységek).
- Leggyakoribb a **Descartes-féle (derékszögű)** rendszer. Egyenes vonalú mozgásnál elég egy tengely (általában *x*, függőleges mozgásnál *y*).
- A tengely nyíl felőli iránya **pozitív**, az ellenkező **negatív**.
- **Vonatkoztatási rendszer:** az egymáshoz képest nyugvó koordinátarendszerek összessége (pl. laborasztalhoz, Naphoz, állócsillagokhoz kötve). Ezekben mérve a test **sebessége és gyorsulása ugyanakkora**.

#### Mértékegységek (SI) és mérés
| Mennyiség | Alapegység | Definíció röviden |
|---|---|---|
| idő | **s** (másodperc) | a cézium-133 atom két meghatározott energiaszintje közti átmenet sugárzása periódusidejének 9 192 631 770-szerese |
| hosszúság | **m** (méter) | az a távolság, amelyet a fény vákuumban $1/299\,792\,458$ s alatt megtesz |

- **Történet röviden:**
  - Az idő mérése régen a Föld forgásán alapult. Az atomórák kimutatták, hogy a forgás kicsit ingadozik, ezért 1967-ben atomi időszabványt fogadtak el.
  - A méter eredetileg a sèvres-i platina-iridium rúd két jelzése közti távolság volt. 1960-ban fényhullámhosszhoz, 1983-ban a fénysebességhez kötötték. Így a méter és a másodperc bármikor reprodukálható, etalon nélkül.
- **Régi egységek:** 1 yd = 0,9144 m (pontosan); 1 in = 2,54 cm (pontosan); 1 Å (angström) $= 10^{-10}$ m; 1 µ (mikron) $= 10^{-6}$ m.
- **Jelölések:**
  - a tudósokról elnevezett egység teljes neve kisbetűs (newton), rövidítése nagybetűs (N);
  - a rövidítés egyes és többes számban ugyanaz, utána nincs pont;
  - két egység együtt: kötőjel a névben, de pont a jelben (newton-méter, N·m);
  - osztás: törtvonal vagy negatív kitevő (m/s vagy m·s⁻¹);
  - sok számjegyű számot hármas csoportokra bontunk (123 456,789 87).
  - Egyenletekben a **vízszintes törtvonalat** használjuk (nem ferdét).

**SI előtagok (prefixumok):**

| Szorzó | Név | Jel | | Szorzó | Név | Jel |
|---|---|---|---|---|---|---|
| $10^{18}$ | exa | E | | $10^{-1}$ | deci | d |
| $10^{15}$ | peta | P | | $10^{-2}$ | centi | c |
| $10^{12}$ | tera | T | | $10^{-3}$ | milli | m |
| $10^{9}$ | giga | G | | $10^{-6}$ | mikro | µ |
| $10^{6}$ | mega | M | | $10^{-9}$ | nano | n |
| $10^{3}$ | kilo | k | | $10^{-12}$ | pico | p |
| $10^{2}$ | hekto | h | | $10^{-15}$ | femto | f |
| $10^{1}$ | deka | da | | $10^{-18}$ | atto | a |

(A hármas lépésközű előtagokat használjuk a leggyakrabban. Kivétel a centi.)

#### Mértékegység-átváltás
- Egy egyenletbe **mindig ugyanazt az egységrendszert** helyettesítsük be (pl. hosszúság: m, idő: s). Méter és kilométer, másodperc és óra nem keverhető.
- **Módszer:** a mért értéket megszorozzuk az egymásnak megfelelő új és régi egység **hányadosaival** (átszámítási tényezők), amelyek értéke 1.
- Példa: $72\ \dfrac{\text{km}}{\text{h}} = 72\cdot\dfrac{1000\ \text{m}}{1\ \text{km}}\cdot\dfrac{1\ \text{h}}{3600\ \text{s}} = 20\ \dfrac{\text{m}}{\text{s}}$
- Gyors szabály: **km/h → m/s: osztunk 3,6-tal; m/s → km/h: szorzunk 3,6-tal.**

#### Normál alak, értékes jegyek
- **Normál alak:** szám $= a\cdot 10^{k}$, ahol $1\le a<10$. Pl. $1926 = 1{,}926\cdot10^{3}$; $0{,}000\,371 = 3{,}71\cdot10^{-4}$. (Számológépen: 1,926 E3.)
- **Értékes jegyek:** a mérés pontosságát mutatják. A 4,2 m két, a 4,20 m három értékes jegyre pontos. Az utolsó leírt jegy már az első bizonytalan jegy. A tizedesvesszőt közvetlenül követő nullák **nem** értékesek ($5\cdot10^{-5}$ egy jegyre pontos).
- Az 1800 m kétértelmű (lehet 2, 3 vagy 4 értékes jegy). **Normál alakkal** egyértelmű: $1{,}8\cdot10^{3}$ (2 jegy) vagy $1{,}800\cdot10^{3}$ (4 jegy).
- **Szabályok számoláskor:**
  - **Összeadás/kivonás:** az eredmény annyi tizedesjegyű, mint a legkevesebb tizedesjegyű tag. Pl. $472 + 3{,}64 = 475{,}64 \to 476$.
  - **Szorzás/osztás:** az eredményben nem lehet több értékes jegy, mint a legkevésbé pontos tényezőben. Pl. $5{,}7624\cdot2{,}60 = 14{,}9$.
  - **Kerekítés:** ha az elhagyott jegy 5-nél kisebb, az utolsó marad. Ha 5 vagy nagyobb, eggyel nő. Kerekíteni csak a **számolás végén** érdemes.
- **A könyv egyszerűsítése:** minden megadott adatot elég pontosnak tekintünk, hogy a végeredményt **3 értékes jegyre** kerekíthessük (pl. a „2 s" számolásnál 2,00 s).
- Bizonytalanság jelölése: pl. $7{,}75 \pm 0{,}04$ m (az igazi érték kb. 2/3 valószínűséggel esik az intervallumba, a könyv 66%-ot ír).

#### Hely, elmozdulás
- **Hely (helykoordináta), $x$:** a pont koordinátája a választott tengelyen.
- **Elmozdulás, $\Delta x$:** a **végső és a kezdeti hely különbsége**. Előjeles mennyiség:
  - pozitív → pozitív irányú elmozdulás, negatív → negatív irányú.
  - **Nem azonos a megtett úttal!** Ha visszaérek a kiindulópontba, az elmozdulás 0, az út nem.
- A $\Delta$ jel mindig *végső − kezdeti* értéket jelent.

#### Átlagsebesség és átlagsebesség-vektor
- **Átlagsebesség (skalár):** a megtett **út** és az ehhez kellő **idő** hányadosa. Nem mond semmit a mozgás irányáról és részleteiről.
- **Átlagsebesség-vektor:** az **elmozdulás** és az eltelt idő hányadosa. Előjele megmutatja az irányt.
- Ez a kettő **nem ugyanaz!** Példa: az indianapolisi 500-as autóverseny győztese 256 km/h átlagsebességet ért el, de az **átlagsebesség-vektora nulla**, mert a cél és a rajt ugyanott van (elmozdulás = 0).
- Az egész mozgás átlagsebessége **nem** a szakaszok átlagsebességeinek átlaga (ha a szakaszok nem tartanak egyenlő ideig).

#### Pillanatnyi sebesség
- Az **adott időpillanatra** vonatkozó sebesség. Úgy kapjuk, hogy az időintervallumot egyre rövidebbre vesszük ($\Delta t \to 0$) és az átlagsebességek **határértékét** nézzük.
- **Szavakban:** a $\Delta x/\Delta t$ különbségi hányados határértéke, amikor $\Delta t$ nullához tart. Ez az $x(t)$ függvény **idő szerinti deriváltja**.
- **Grafikus jelentés:** az $x(t)$ grafikon adott pontjához húzott **érintő iránytangense (meredeksége)**.
  - Az érintő lefelé lejt → a sebesség negatív.
  - Az érintő vízszintes (a görbe csúcsán) → a sebesség nulla (itt fordul meg a test).
- A pillanatnyi sebesség **abszolút értéke** a skaláris pillanatnyi sebesség. Gyakran csak „sebességet" mondunk, a szövegkörnyezetből kiderül, melyikre gondolunk. (Angolul két külön szó van: *speed* és *velocity*.)

#### Gyorsulás
- **Átlagos gyorsulás:** a sebesség megváltozása osztva az eltelt idővel. Megmutatja, mennyit változik a sebesség **időegység** alatt.
- **Pillanatnyi gyorsulás:** az átlagos gyorsulás határértéke ($\Delta t\to0$), vagyis a sebesség idő szerinti deriváltja. Ez az $x(t)$ **második deriváltja**. Grafikusan: a $v(t)$ grafikon érintőjének meredeksége.
- A gyorsulás mind a gyorsulást, mind a **lassulást** magában foglalja.
- **Mikor gyorsul / lassul a test?** (Figyeljük a *v* és *a* előjelét!)
  - *v* és *a* **azonos előjelű** → a test **gyorsul** (a sebesség nagysága nő).
  - *v* és *a* **ellentétes előjelű** → a test **lassul**.
  - Példa: $v>0$, $a<0$ → a test pozitív irányban lassulva mozog.

#### Hamis gyökök
- Ha a feladat másodfokú egyenletre vezet (pl. az idő az ismeretlen), két gyököt kapunk. **Mindkettőt meg kell vizsgálni fizikailag.**
- A negatív idő például a mozgás kezdete *előtti* időpont. Ott a kinematikai egyenletek nem érvényesek, ezért ez **hamis gyök**, el kell vetni.
- Ha mindkét gyök értelmes (pl. felfelé és visszafelé is áthalad a labda ugyanazon a magasságon), akkor mindkettő jó megoldás.

#### Dimenzióanalízis
- Egy fizikai egyenletben csak **azonos dimenziójú** tagok szerepelhetnek (nem adhatunk össze almát és autót).
- **Dimenzió ≠ mértékegység:** a hosszúság dimenziója $L$ (mértékegysége lehet m, km...), az időé $T$.
  - $[x]=L$, $[v]=L/T$, $[a]=L/T^2$
- A számszerű együtthatóknak (pl. $\tfrac12$) nincs dimenziójuk, elhagyhatók.
- Ellenőrzés példa: $x = x_0 + v_0 t + \tfrac12 a t^2 \Rightarrow [L] = [L] + \dfrac{L}{T}\cdot T + \dfrac{L}{T^2}\cdot T^2 = [L]+[L]+[L]$ ✔
- **Haszna:** hibakeresésre jó. Ha a dimenziók nem egyeznek, biztosan hibáztunk. Ha egyeznek, az még **nem** garantálja, hogy a számolás helyes.

---

### 2.2 Képletek

#### Alapdefiníciók

| Képlet | Jelek | Mértékegység |
|---|---|---|
| $\Delta x = x_2 - x_1$ | $\Delta x$: elmozdulás; $x_2$: végső hely; $x_1$: kezdeti hely | m |
| $v_{\text{átl,sk}} = \dfrac{\text{összes út}}{\text{összes idő}}$ | átlagsebesség (skalár) | m/s |
| $v_{\text{átl}} = \dfrac{\Delta x}{\Delta t} = \dfrac{x_2 - x_1}{t_2 - t_1}$ | $v_{\text{átl}}$: átlagsebesség-vektor; $\Delta t$: eltelt idő | m/s |
| $v = \lim\limits_{\Delta t\to0}\dfrac{\Delta x}{\Delta t} = \dfrac{dx}{dt}$ | $v$: pillanatnyi sebesség | m/s |
| $a_{\text{átl}} = \dfrac{\Delta v}{\Delta t} = \dfrac{v_2 - v_1}{t_2 - t_1}$ | $a_{\text{átl}}$: átlagos gyorsulás; $\Delta v$: sebességváltozás | m/s² |
| $a = \lim\limits_{\Delta t\to0}\dfrac{\Delta v}{\Delta t} = \dfrac{dv}{dt} = \dfrac{d^2x}{dt^2}$ | $a$: pillanatnyi gyorsulás | m/s² |

A **hatványfüggvény deriválási szabálya**, amelyet a fejezet használ:

$$x = C\,t^{n} \;\Rightarrow\; v = \frac{dx}{dt} = n\,C\,t^{\,n-1}$$

Az **integrálási szabály** (ennek fordítottja): $\displaystyle\int t^{n}\,dt = \frac{t^{n+1}}{n+1} + C$

#### Egyenletesen gyorsuló egyenesvonalú mozgás (a = állandó) kinematikai egyenletei

| Sorszám | Képlet | Mi hiányzik belőle? | Használd, ha... |
|---|---|---|---|
| (2-11) | $v = v_0 + a\,t$ | $x$ | nem kell/nem ismert a hely |
| (2-12) | $x = x_0 + v_0\,t + \tfrac12 a\,t^2$ | $v$ | nem kell/nem ismert a végsebesség |
| (2-13) | $v^2 = v_0^2 + 2a\,(x - x_0)$ | $t$ | **nem ismert az idő** |
| (2-14) | $v_{\text{átl}} = \dfrac{v_0 + v}{2}$ | $a$, $x$ | (csak állandó gyorsulásnál!) |
| (2-15) | $x = x_0 + v_{\text{átl}}\,t$ | $a$ | nem ismert a gyorsulás |

**Jelek:**
- $x$: a hely $t$ időpontban (m); $x_0$: kezdeti hely $t=0$-nál (m)
- $v$: sebesség $t$ időpontban (m/s); $v_0$: kezdősebesség (m/s)
- $a$: (állandó) gyorsulás (m/s²); $t$: idő (s)
- Függőleges mozgásnál $x$ helyett $y$-t írunk.

**Szabadesés / hajítás:** a gravitációs gyorsulás $g = 9{,}81\ \text{m/s}^2$ (3 értékes jegyre), iránya mindig **lefelé**.
- Ha a **felfelé** mutató irányt választjuk pozitívnak: $a = -g$.
- Ha a **lefelé** mutatót: $a = +g$.
- (A feladatok egy részében a könyv $g = 10\ \text{m/s}^2$-tel számol, ezt mindig jelzi a feladat.)

**Előjel-megjegyzés:** a kinematikai egyenleteket **mindig pontosan ebben az alakban** írjuk fel, bármelyik irányt választjuk pozitívnak. A választás csak az adatok előjelét befolyásolja.

**Egyszerűsítés:** ha az origót oda tesszük, ahol a test $t=0$-ban van, akkor $x_0 = 0$ és eggyel kevesebb ismeretlen marad.

**Ezek az egyenletek csak állandó gyorsulásnál érvényesek!** Ha $a$ az időben változik, integrálással kell számolni (lásd 2-6, 2-7 példa).

#### Diákmankó (háromszögek)

Takard le azt, amit keresel! Ami marad, az megmutatja a műveletet. Egymás mellett: **szorzás**, egymás felett: **osztás**.

```
        átlagsebesség-vektor / egyenletes mozgás          gyorsulás / sebességváltozás

              /\                                                /\
             /  \                                              /  \
            / s  \                                            / Δv \
           /------\                                          /------\
          / v | t  \                                        / a | t  \
         /__________\                                      /__________\

   s = v · t     v = s / t     t = s / v          Δv = a · t    a = Δv / t    t = Δv / a
```

Az első háromszög állandó sebességnél, vagy az átlagsebességgel számolva ($s = v_{\text{átl}}\cdot t$) használható.

**„Melyik egyenletet használjam?"**, a hiányzó mennyiség alapján:

| Ha NEM ismert / nem kell... | ...akkor ezt használd |
|---|---|
| a végsebesség $v$ | $x = x_0 + v_0 t + \tfrac12 a t^2$ |
| a hely $x$ | $v = v_0 + a t$ |
| az idő $t$ | $v^2 = v_0^2 + 2a(x - x_0)$ |
| a gyorsulás $a$ | $x = x_0 + \tfrac12(v_0 + v)\,t$ |

#### Levezetések

**(a) $v = v_0 + a t$ (2-11)**
- Állandó gyorsulásnál az átlagos és a pillanatnyi gyorsulás megegyezik:
  $a = \dfrac{\Delta v}{\Delta t} = \dfrac{v - v_0}{t - 0}$
- Átrendezve: $v = v_0 + a t$ ✔

**(b) $x = x_0 + v_0 t + \tfrac12 a t^2$ (2-12), grafikusan**
- Rajzoljuk fel a $v(t)$ egyenest. A görbe alatti terület az **elmozdulás**.
- A terület két részre bontható:
  - alsó **téglalap**: $v_0\cdot t$
  - felső **háromszög**: $\tfrac12 (v - v_0)\,t$
- Összeadva: $v_0 t + \tfrac12(v - v_0)t = \dfrac{v_0 + v}{2}\,t$. Ez az átlagsebesség és az idő szorzata.
- Állandó $a$ miatt $v_{\text{átl}} = \dfrac{v_0 + v}{2}$ és $\Delta x = v_{\text{átl}}\, t$, vagyis $x - x_0 = \dfrac{v_0+v}{2}\,t$ (2-8).
- Behelyettesítve $v = v_0 + a t$-t: $x - x_0 = v_0 t + \tfrac12 a t^2$ ✔

**(b') Ugyanez integrálással**
- $x = \int v\,dt = \int (v_0 + a t)\,dt = v_0 t + \tfrac12 a t^2 + C_2$
- A $C_2$ integrálási állandót a kezdeti feltétel adja: $t=0$-nál $x = x_0$, tehát $C_2 = x_0$ ✔
- (A grafikus és az analitikus levezetés lényegében ugyanaz, mert az integrál geometriai jelentése a görbe alatti terület.)

**(c) $v^2 = v_0^2 + 2a(x - x_0)$ (2-13)**
- Kiküszöbölve az időt a (2-11) és (2-12) egyenletekből (tisztán algebrai átalakítás) kapjuk.

**(d) Az első egyenlet integrálással**
- $a = \dfrac{dv}{dt} \Rightarrow dv = a\,dt \Rightarrow v = \int a\,dt = a t + C_1$
- Kezdeti feltétel: $t = 0$-nál $v = v_0$, így $C_1 = v_0$ → $v = v_0 + at$ ✔

#### Grafikonok kapcsolata (2.9)

| Grafikon | Meredekség | Görbe alatti terület |
|---|---|---|
| $x(t)$ | = $v$ (pillanatnyi sebesség) | – |
| $v(t)$ | = $a$ (gyorsulás) | = $\Delta x$ (elmozdulás) |
| $a(t)$ | – | = $\Delta v$ (sebességváltozás) |

- **Deriválás irányába:** $x(t) \to v(t) \to a(t)$ (meredekség).
- **Integrálás irányába:** $a(t) \to v(t) \to x(t)$ (terület).
- Az integrálásnál a **kezdeti feltétel** ($x_0$, $v_0$) nem adódik a grafikonból, ezeket külön meg kell adni.
- Ha a $v(t)$ görbe a $t$ tengely **alatt** van, a hozzá tartozó terület negatív: az elmozdulás ilyenkor csökken.
- Állandó gyorsulás → $v(t)$ **egyenes**, $x(t)$ **parabola**.

---

### 2.3 Feladatok levezetése (a fejezet példái)

#### 2-1 példa: kocogó atléta
*Egy atléta egyenes úton kocogva 30 perc alatt 6 km-t tesz meg, majd megfordul és 20 perc alatt 2 km-t visszagyalogol. Határozzuk meg: a) az elmozdulást, b) az átlagsebességet, c) az átlagsebesség-vektort a teljes úton, d) az átlagsebesség-vektort a kocogás, e) a gyaloglás szakaszán.*

**Felvett adatok:** $x_0 = 0$ ($t_0 = 0$), $x_1 = 6$ km ($t_1 = 30$ perc), $x_2 = 4$ km ($t_2 = 50$ perc).

- **a)** $\Delta x = x_2 - x_0 = 4\ \text{km} - 0 = 4\ \text{km}$
- **b)** Összes út $= 6 + 2 = 8$ km, összes idő $= 30 + 20 = 50$ perc
  $$v_{\text{átl,sk}} = \frac{8\ \text{km}}{50\ \text{perc}} = 0{,}160\ \frac{\text{km}}{\text{perc}}$$
- **c)** $v_{\text{átl}} = \dfrac{\Delta x}{\Delta t} = \dfrac{4\ \text{km} - 0}{50\ \text{perc} - 0} = 0{,}080\ \dfrac{\text{km}}{\text{perc}}$
- **d)** Kocogás: $v_{\text{átl}} = \dfrac{x_1 - x_0}{t_1 - t_0} = \dfrac{6\ \text{km}}{30\ \text{perc}} = 0{,}200\ \dfrac{\text{km}}{\text{perc}}$
- **e)** Gyaloglás: $v_{\text{átl}} = \dfrac{x_2 - x_1}{t_2 - t_1} = \dfrac{4 - 6\ \text{km}}{50 - 30\ \text{perc}} = \dfrac{-2\ \text{km}}{20\ \text{perc}} = -0{,}100\ \dfrac{\text{km}}{\text{perc}}$
  - A **negatív előjel** azt jelenti, hogy a sebesség iránya $-x$.

**Tanulság:** a két szakasz átlagsebesség-vektorának számtani közepe **nem** adja a teljes útra vett értéket, mert a két szakasz nem egyenlő ideig tartott. Mindig *végső − kezdeti* értékkel számolunk.

#### 2-2 példa: átlagsebesség egy konkrét mozgásnál
*Egy test helye $x = 10t^2$ (x méterben, t másodpercben). Határozzuk meg az átlagsebesség-vektort a) 2 s és 3 s között, b) 2,0 s és 2,1 s között.*

- $t_1 = 2{,}0$ s → $x_1 = 10\cdot2^2 = 40$ m; $t_3 = 3{,}0$ s → $x_3 = 10\cdot3^2 = 90$ m
- **a)** $v_{\text{átl}} = \dfrac{90 - 40\ \text{m}}{3 - 2\ \text{s}} = \dfrac{50\ \text{m}}{1\ \text{s}} = 50{,}0\ \dfrac{\text{m}}{\text{s}}$
- **b)** $t_2 = 2{,}1$ s → $x_2 = 10\cdot(2{,}1)^2 = 44{,}1$ m
  $$v_{\text{átl}} = \frac{44{,}1 - 40\ \text{m}}{2{,}1 - 2{,}0\ \text{s}} = \frac{4{,}1\ \text{m}}{0{,}1\ \text{s}} = 41{,}0\ \frac{\text{m}}{\text{s}}$$
- **Megfigyelés:** minél rövidebb az időintervallum, annál közelebb vagyunk a $t = 2$ s-hoz tartozó pillanatnyi sebességhez (a következő példa szerint 40 m/s).

#### 2-3 példa: a derivált definíciója a gyakorlatban
*Határozzuk meg az $x = 10t^2$ mozgás pillanatnyi sebességét a határértékképzéssel.*

- Legyen $x_1 = 10t_1^2$ és $t_2 = t_1 + \Delta t$:
  $$x_2 = 10(t_1 + \Delta t)^2 = 10\left[t_1^2 + 2t_1\Delta t + (\Delta t)^2\right]$$
- Elmozdulás: $\Delta x = x_2 - x_1 = 20\,t_1\,\Delta t + 10(\Delta t)^2$
- Különbségi hányados: $\dfrac{\Delta x}{\Delta t} = 20\,t_1 + 10\,\Delta t$
- Ha $\Delta t \to 0$, a második tag eltűnik: $v_1 = \lim\limits_{\Delta t\to0}\dfrac{\Delta x}{\Delta t} = 20\,t_1$
- Mivel $t_1$-re semmilyen kikötést nem tettünk, ez **bármely időpontra** igaz: $\boxed{v = 20t}$
- Ellenőrzés: $t = 2$ s-nál $v = 40{,}0$ m/s ✔ (a 2-2 példában a $2{,}0$–$2{,}1$ s intervallumra 41,0 m/s jött ki, ami közel van).
- **Általános szabály:** $x = Ct^n \Rightarrow v = nCt^{n-1}$. A $v(t)$ itt egyenes, $x(t)$ parabola.

#### 2-4 példa: gyorsulás a sebesség–idő grafikonról
*A $v(t)$ grafikon: 0–2 s között 0-ról 2 m/s-ra nő lineárisan, 2–4 s között állandó (2 m/s), 4–5 s között 2 m/s-ról 0-ra csökken. Rajzoljuk fel $a(t)$-t!*

A gyorsulás a $v(t)$ meredeksége, lineáris szakaszokon a különbségi hányados:
- **0–2 s:** $a_1 = \dfrac{\Delta v}{\Delta t} = \dfrac{2 - 0\ \text{m/s}}{2 - 0\ \text{s}} = 1\ \dfrac{\text{m}}{\text{s}^2}$
- **2–4 s:** $v$ állandó, a meredekség 0 → $a = 0$
- **4–5 s:** $a_2 = \dfrac{0 - 2\ \text{m/s}}{5 - 4\ \text{s}} = -2\ \dfrac{\text{m}}{\text{s}^2}$ (lassulás)

Az $a(t)$ grafikon tehát lépcsős: $+1$ (0–2 s), $0$ (2–4 s), $-2$ (4–5 s).

#### 2-5 példa: elejtett labda, amikor a sebessége 4,9 m/s
*Kezdősebesség nélkül elejtünk egy labdát. A gravitációs gyorsulás 9,81 m/s². Hol van a labda, amikor a sebessége 4,9 m/s? Oldjuk meg úgy, hogy a felfelé, majd úgy, hogy a lefelé irányt választjuk pozitívnak.*

Tudjuk: $y_0 = 0$, $v_0 = 0$, $|v| = 4{,}9$ m/s, keressük $y$-t. Az idő nem kell → **(2-13)**: $v^2 = v_0^2 + 2a(y - y_0)$.

| | **Felfelé pozitív** | **Lefelé pozitív** |
|---|---|---|
| $a$ | $-9{,}81$ m/s² | $+9{,}81$ m/s² |
| $v$ | $-4{,}9$ m/s (lefelé mozog) | $+4{,}9$ m/s |
| behelyettesítés | $(-4{,}9)^2 = 0 + 2(-9{,}81)\,y$ | $(4{,}9)^2 = 0 + 2(9{,}81)\,y$ |
| $y = \dfrac{v^2}{2a}$ | $\dfrac{24{,}0}{-19{,}62} = -1{,}22$ m | $\dfrac{24{,}0}{19{,}62} = +1{,}22$ m |
| jelentés | a negatív előjel: a kiindulás **alatt** | a pozitív előjel: a kiindulás **alatt** |

**Tanulság:** a fizikai eredmény ugyanaz (a labda **1,22 m-rel a kiindulópont alatt** van). Az előjel csak a tengely irányának választását tükrözi. A képlet a választástól függetlenül érvényes.

#### 2-6 példa: $x = 4t^3$, sebesség és gyorsulás deriválással
*Egy részecske helyzete $x = 4t^3$ (m, s). Mekkora a sebessége és a gyorsulása $t = 2$ s-nál?*

- **a)** $v = \dfrac{dx}{dt} = \dfrac{d}{dt}(4t^3) = 12\,t^2$ → $t = 2$ s: $v = 12\cdot 4 = 48{,}0$ m/s
  (a 12 együttható mértékegysége m/s³, hogy a dimenzió stimmeljen)
- **b)** $a = \dfrac{dv}{dt} = \dfrac{d}{dt}(12t^2) = 24\,t$ → $t = 2$ s: $a = 48$ m/s²

#### 2-7 példa: változó gyorsulás integrálással
*Egy rakéta gyorsulása $a = 3t + 5$ (SI). Milyen messzire jut el $t = 2$ s alatt? (Indulás: $x_0 = 0$, $v_0 = 0$.)*

- $a = \dfrac{dv}{dt} \Rightarrow dv = a\,dt$; integrálva:
  $$v = \int_0^t (3t+5)\,dt = \frac{3t^2}{2} + 5t$$
- $v = \dfrac{dx}{dt} \Rightarrow dx = v\,dt$; integrálva:
  $$x = \int_0^t\left(\frac{3t^2}{2} + 5t\right)dt = \frac{t^3}{2} + \frac{5t^2}{2}$$
- $t = 2$ s: $x = \dfrac{8}{2} + \dfrac{5\cdot4}{2} = 4 + 10 = \boxed{14{,}0\ \text{m}}$
- Itt a kezdeti feltétel miatt mindkét integrálási állandó 0.

#### 2-8 példa: felfelé hajított labda szakadék szélén
*Egy labdát 20 m/s-mal felfelé hajítunk egy szakadék széléről, $g = 10$ m/s². a) Milyen magasra emelkedik? b) Mennyi idő múlva lesz 25 m-rel a kiindulási hely alatt?*

**Módszer (4 lépés):** feladattípus felismerése → vázlat → adatok csoportosítása → megfelelő egyenlet kiválasztása.
- A labda állandó gyorsulású egyenesvonalú mozgást végez → alkalmazhatók a kinematikai egyenletek.
- Koordinátarendszer: $y$ felfelé pozitív, origó az elhajítás helye: $y_0 = 0$, $v_0 = 20$ m/s, $a = -10$ m/s².

**a)** A csúcspontban $v = 0$. Az idő nem kell → (2-13):
$$y = \frac{v^2 - v_0^2}{2a} + y_0 = \frac{0 - (20)^2}{2\cdot(-10)} + 0 = \boxed{20\ \text{m}}$$

**b)** Most $y = -25$ m, az ismeretlen $t$ (és $v$ nem ismert). A (2-12) egyenletet használjuk. **A mozgást nem kell két részre bontani** (fel, majd le), mert a kinematikai egyenletek akkor is érvényesek, ha a labda csak a gravitáció hatására mozog, akár felfelé, akár lefelé.
$$y = y_0 + v_0 t + \tfrac12 a t^2 \Rightarrow -25 = 20t - 5t^2$$
Rendezve: $5t^2 - 20t - 25 = 0 \Rightarrow t^2 - 4t - 5 = 0 \Rightarrow (t - 5)(t + 1) = 0$
- $t = 5$ s ✔
- $t = -1$ s ✘ → **hamis gyök** (a mozgás kezdete előtti időpont, nincs fizikai értelme).

$$\boxed{t = 5{,}00\ \text{s}}$$

#### 2-9 példa: fékező autó
*Egy gépkocsi 54 km/h sebességről egyenletesen lefékez. a) Mekkora utat tesz meg a fékezés első 2 s-ában? b) Mekkora a sebessége 2 s végén? c) Mennyi idő alatt áll meg? d) Mekkora a teljes fékút?*

> ⚠️ **Eltérés a könyvben (ellenőrizd a nyomtatott könyvben!):** a feladat szövege (a beolvasott PDF-ben) 4 m/s² lassulást írhat, a **megoldás viszont végig 5 m/s²-tel számol** (ezekkel jön ki a 20 m, 5 m/s, 3 s, 22,5 m). Lehet nyomdahiba vagy beolvasási hiba. Lent a megoldás 5 m/s²-es értékeivel számolok.

- Átváltás: $v_0 = 54\ \dfrac{\text{km}}{\text{h}} = 54\cdot\dfrac{1}{3{,}6} = 15\ \dfrac{\text{m}}{\text{s}}$
- Lassul → $a = -5\ \text{m/s}^2$ (negatív); $x_0 = 0$.

- **a)** $x_1 = v_0 t_1 + \tfrac12 a t_1^2 = 15\cdot2 + \tfrac12(-5)(2)^2 = 30 - 10 = \boxed{20\ \text{m}}$
- **b)** $v_1 = v_0 + a t_1 = 15 + (-5)\cdot2 = \boxed{5\ \dfrac{\text{m}}{\text{s}}}$
- **c)** Megálláskor $v_2 = 0$: $t_2 = \dfrac{v_2 - v_0}{a} = \dfrac{0 - 15}{-5} = \boxed{3\ \text{s}}$
- **d)** (2-13)-ból: $x_2 = \dfrac{v_2^2 - v_0^2}{2a} = \dfrac{0 - 225}{2\cdot(-5)} = \boxed{22{,}5\ \text{m}}$

#### 2-10 példa: motoros és rendőr (utolérés)
*Egy motoros 180 km/h-val száguld az autópályán (a megengedett 120 km/h). A rendőr abban a pillanatban, amikor a motoros elhalad mellette, nyugalomból indul $a = 5$ m/s² gyorsulással. Mennyi idő alatt éri utol?*

- Átváltás: $v_M = 180/3{,}6 = 50$ m/s (állandó, $a_M = 0$); a rendőr: $v_{P0} = 0$, $a_P = 5$ m/s².
- **A döntő felismerés (vázlat!):** utolérésnél a két test **ugyanott** van és **ugyanannyi ideig** mozgott (ugyanonnan és ugyanakkor indultak) → az elmozdulások egyenlők: $x_M = x_P$.
- Felírjuk (2-12)-t mindkettőre ($x_0 = 0$):
  $$v_{M0}\,t + \tfrac12 a_M t^2 = v_{P0}\,t + \tfrac12 a_P t^2$$
  $$50\,t + 0 = 0 + \tfrac12\cdot5\,t^2$$
- Rendezve: $t\left(50 - 2{,}5\,t\right) = 0 \Rightarrow t = 0$ (a kezdet) vagy $t = \dfrac{50}{2{,}5}$:
  $$\boxed{t = 20\ \text{s}}$$
- (Kiegészítés: ekkor a rendőr sebessége $5\cdot20 = 100$ m/s, és mindketten $50\cdot20 = 1000$ m-re vannak az útjelző táblától.)

**Tanulság:** a vázlat segít észrevenni, hogy az elmozdulások és az idők megegyeznek. Ez kulcs a megoldáshoz.

---

### 2.4 Egyszerű módja a téma megértésének

**Képzeld el az autódat:**
- A **kilométeróra** a **pillanatnyi sebesség** ($v = dx/dt$): éppen most mennyivel mész.
- Az **útitervező átlaga** az **átlagsebesség**: összes út / összes idő. Hazaértél a kiindulási pontra? Az átlagsebesség-*vektor* 0.
- A **gázpedál** a **gyorsulás**: azt mondja meg, mennyire gyorsan változik a kilométeróra állása.

**A három mennyiség egy láncot alkot:**
```
   hely  x   ──(deriválás: meredekség)──▶   sebesség  v   ──(deriválás)──▶   gyorsulás  a
   hely  x   ◀──(integrálás: terület)────   sebesség  v   ◀──(integrálás)──   gyorsulás  a
```

**Grafikonolvasás 3 mondatban:**
1. Az $x(t)$ grafikon **meredeksége** = sebesség (felfelé tart → +, lefelé → −, vízszintes → áll).
2. A $v(t)$ grafikon **meredeksége** = gyorsulás, a **görbe alatti terület** = megtett elmozdulás.
3. Az $a(t)$ grafikon **görbe alatti területe** = sebességváltozás.

**Előjelek:**
- $v$ és $a$ **azonos** előjelű → gyorsul. **Ellentétes** → lassul.
- Pozitív $a$ nem azt jelenti, hogy gyorsul! Csak ha $v$ is pozitív.

**Feladatmegoldási recept (a könyv szerint):**
1. **Feladattípus:** ha állandó $a$ → kinematikai egyenletek.
2. **Vázlat:** origó, pozitív irány, jelölések, fontos pontok.
3. **Adatok csoportosítása**, azonos mértékegységrendszerben (szükség esetén átváltás!).
4. **Egyenlet kiválasztása** a hiányzó mennyiség alapján (lásd a táblázatot fent). Ha az origót a kezdőponthoz tesszük, $x_0$ kiesik.
5. **Ellenőrzés:** van-e értelme az eredménynek? Furcsa érték hibára utalhat. Másodfokúnál vizsgáld meg mindkét gyököt (hamis gyök!).
6. **Dimenzióellenőrzés** is segít a hibák felderítésében.

**Gyakori hibák:**
- Út és elmozdulás összekeverése.
- Átlagsebesség ≠ a két végsebesség átlaga (általában!). Csak **állandó gyorsulásnál** igaz, hogy $v_{\text{átl}} = (v_0 + v)/2$.
- km/h és m/s keverése egy egyenleten belül.
- Az előjel figyelmen kívül hagyása szabadesésnél ($a = -g$, ha felfelé a pozitív).

---

## 3. Téma lezárása

### Rövid emlékeztető: mit tanultunk?
- A **kinematika** a mozgás leírása (hol? mikor?), az okok nélkül. A testet **anyagi pontnak** tekintjük.
- Egy mozgást **koordinátarendszerben/vonatkoztatási rendszerben** írunk le. Az **SI** mértékegységeket használjuk, ügyelve az átváltásra és az **értékes jegyekre**.
- **Hely** → **elmozdulás** ($\Delta x$, előjeles) → **sebesség** ($v = dx/dt$) → **gyorsulás** ($a = dv/dt$).
- **Átlagsebesség** (út/idő) ≠ **átlagsebesség-vektor** (elmozdulás/idő).
- **Állandó gyorsulásnál** három fő egyenlet: $v = v_0 + at$, $x = x_0 + v_0 t + \tfrac12 at^2$, $v^2 = v_0^2 + 2a(x-x_0)$. A hiányzó mennyiség dönti el, melyiket használjuk.
- A kinematikai egyenletek **deriválással/integrálással** vezethetők le, és a grafikonokon **meredekség ↔ terület** kapcsolat van közöttük.
- **Szabadesés/hajítás:** $a = \pm g$ ($g = 9{,}81$ m/s²).
- Ellenőrzési eszközök: **dimenzióanalízis** és a **hamis gyökök** vizsgálata.

### Rövid befejezés
Ezzel megvan a mozgástan alapnyelve. A fejezet példái megmutatták, hogy egy jó vázlat és a hiányzó mennyiség alapján választott egyenlet a legtöbb feladatot megoldja. A következő lépés: ugyanezt kiterjeszteni két és három dimenzióra, ahol a hely, a sebesség és a gyorsulás már **vektorok** lesznek, és megjelennek az összetett mozgások (pl. ferde hajítás).

### Gyakorló feladatok a fejezet végén (a könyvből)
| Alfejezet | Feladatok |
|---|---|
| 2.3 Mértékegységek átszámítása | 2A-1 … 2B-10 |
| 2.5 Hely, elmozdulás, sebesség | 2A-11 … 2B-19 |
| 2.6 Gyorsulás | 2A-20 … 2B-26 |
| 2.7 Egyenletesen gyorsuló mozgás | 2A-27 … 2B-38 |
| 2.8 Levezetés differenciálszámítással | 2B-39 … 2B-41 |
| 2.9 Grafikus értelmezés | 2B-42 … 2B-45 |
| 2.10 Dimenzióanalízis | 2A-46 … 2B-48 |
| További feladatok | 2C-49 … 2C-66 |

A kérdések (1–12) fogalmi gyakorlásra valók. A **páratlan sorszámú feladatok** megoldása a könyv végén található (az „1–23 fejezetek páratlan számozású feladatainak megoldásai" rész, II. fejezet).

### ➡️ Következő modul
**Síkbeli és térbeli mozgás:** [[sikbeli_es_terbeli_mozgas]]
