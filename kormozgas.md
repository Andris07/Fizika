# Körmozgás

> Forrás: a könyv IV. fejezete (4.1–4.4 + Összefoglalás, Kérdések, Feladatok).
> Az előző modul vektoros leírását használjuk fel egy különleges, nagyon gyakori síkmozgásra: a körpályán való mozgásra.

---

## 1. Téma bevezetése

### Mi a téma?
Körpályán mozgó test (részecske) helyzetének, sebességének és gyorsulásának leírása. A fejezet végén kitekintés az **általános görbe vonalú mozgásra** is.

### Mi a téma jelentése?
- A körmozgás az egyik **legfontosabb síkmozgás**, ezért külön, kényelmes jelölési rendszert dolgozunk ki hozzá (síkbeli polárkoordináták).
- **A fejezet legfontosabb, meglepő felismerése:** az egyenletes sebességgel körpályán mozgó test sebességének **nagysága** nem változik, **mégis gyorsul**.
  - Ez első pillantásra érthetetlennek tűnik, de a gyorsulás definíciójából ($\mathbf a = d\mathbf v/dt$) azonnal következik: ha a sebességvektor **iránya** folytonosan változik, a sebességvektor változik, tehát van gyorsulás.
- Két gyorsulás-összetevő különböztethető meg: az **érintő menti (tangenciális)** és a **sugár irányú (centripetális)**.

### Mindennapi előfordulás, felhasználás
- **A könyv példái:** gépek forgórészei, kanyarodó autó, a Bohr-modell szerint a hidrogénatom elektronjai, a Föld körül keringő mesterséges holdak.
- **További példák a fejezet feladataiból:** lemezjátszó korongja, vidámparki körhinta és óriáskerék, centrifuga, fogorvosi fúró, helikopter légcsavarja, a Hold keringése, a Föld forgása, a versenypálya kanyarja, repülő sólyom.
- **Fizikában:** a körmozgás leírása és a centripetális gyorsulás szükséges az erők, a bolygómozgás, a gravitáció és a mágneses mezőben mozgó töltött részecskék tárgyalásához.

---

## 2. Téma kifejtése

### 2.1 Alapfogalmak

#### Síkbeli polárkoordináták
- A $P$ pont helyét az origótól mért **$r$ távolsággal** és a **pozitív $x$ tengelytől az óramutató járásával ellentétes irányban mért $\theta$ szöggel** adjuk meg.
- **Körmozgásnál $r$ állandó** (a kör sugara), csak $\theta$ változik az időben. Ezért a polárkoordináták sokkal alkalmasabbak a körmozgás leírására, mint a derékszögűek.
- $\theta$-t **szögkoordinátának** nevezzük. A kinematikai egyenletekben **mindig radiánban** mérjük.

#### Radián
- Egy szög radiánban mért értéke a szöghöz tartozó **körív hosszának és a kör sugarának hányadosa**:
  $$\theta = \frac{s}{r}\quad\text{(radiánban)}$$
- **1 radián:** az a szög, amely alatt a kör középpontjából az az $s$ ív látszik, amelynek hossza a kör sugarával egyenlő.
- Mivel két hosszúság hányadosa, a radián **dimenzió nélküli** egység.
- Egy teljes fordulat: $2\pi$ rad $= 360^\circ$, ebből $1\ \text{rad} = \dfrac{360^\circ}{2\pi} \approx 57{,}3^\circ$.

#### Periódusidő
- **Periódusidő ($T$):** az egy fordulat megtételéhez szükséges idő. Az egyenletes körmozgás ismétlődő (periodikus) mozgás.

#### Érintő menti (tangenciális) gyorsulás
- A **sebességvektor mindig a kör érintőjének irányába mutat**.
- A sebesség **nagyságának** változását leíró gyorsulásösszetevő: $a_t = \dfrac{dv}{dt}$. Mindig a **pálya érintője mentén** van.
- Ha a test **gyorsul**, $a_t$ a mozgás irányába mutat. Ha **lassul**, $a_t$ ellentétes a mozgás irányával. Ha a sebesség **állandó**, $a_t = 0$.
- Szemléletesen: mintha egy egyenes pályát körré hajlítanánk.
- Figyelem: az $a_t = dv/dt$ egyenlet **nem vektoregyenlet**, de tudjuk, hogy az összetevő mindig az érintő irányába mutat.

#### Centripetális (sugár irányú, normális) gyorsulás
- A másik gyorsulásösszetevő **merőleges a pályára**, és mindig a **kör középpontja felé**, azaz **sugár irányban befelé** mutat. Ezt nevezzük **centripetális gyorsulásnak** ($a_{cp}$).
- Az elnevezés eredete: *centrum* (közép) + *petere* (befelé irányulni, törekedni).
- **Ne tévesszük össze a centrifugális gyorsulással** (*fugere* = menekülni, elfutni), amely **radiálisan kifelé** mutat. (A centrifugálisról a könyv a 14. fejezetben ír részletesebben.)

#### Egyenletes körmozgás
- A test **állandó sebességnagysággal** mozog körpályán.
- A centripetális gyorsulás $a_{cp} = \dfrac{v^2}{r}$, **a gyorsulás mindig a kör középpontja felé mutat**, és **merőleges a sebességvektorra**.
- A test mégsem kerül közelebb a középponthoz, bár mindig afelé gyorsul.
- Az érintő menti gyorsulás nulla.

#### Nem egyenletes körmozgás
- Ha a sebesség nagysága is változik (nő vagy csökken), **mindkét** gyorsulásösszetevő fellép: a tangenciális $a_t = dv/dt$ és a centripetális $a_{cp} = v^2/r$.
- A két összetevő **merőleges egymásra**. Az eredő gyorsulás nagysága Pitagorasz-tétellel adódik.
- A gyorsulásvektor ilyenkor **sem a sebesség, sem a sugár irányába nem mutat** (csak a kettő közötti irányba).
- **Általános következtetés:** görbe pályán mozgó test gyorsulásvektora **soha nem lehet azonos irányú a sebességvektorral**.

#### Egységvektorok körmozgásnál: $\hat{\mathbf r}$ és $\hat{\boldsymbol\theta}$
- $\hat{\mathbf r}$: mindig **radiálisan kifelé** mutat (a középponttól a test felé).
- $\hat{\boldsymbol\theta}$: a **pálya érintőjébe** esik, és a $\theta$ szög **növekedésének irányába** mutat (a +x tengelytől az óramutató járásával ellentétes irányba haladva).
- Ezek az egységvektorok **„együtt mozognak" a részecskével**, tehát irányuk a mozgás során változik (nyugvó koordinátarendszerhez képest).
- A centripetális összetevő előtt **negatív előjel** áll, mert a gyorsulás befelé mutat, $\hat{\mathbf r}$ pedig kifelé.

#### Általános görbe vonalú mozgás
- Tetszőleges görbe pálya **bármely pontjában** értelmezhető egy **görbületi kör**, amely az adott pontban a legjobban simul a pályához.
  - A görbületi kör **sugara** a pálya **pillanatnyi görbületi sugara**, a **középpontja** a **görbületi középpont**.
  - (Fordítói megjegyzés a könyvben: a görbületi kör a pontban **másodrendűen** érinti a görbét, azaz az első és a második deriváltjuk megegyezik.)
- Ha ismerjük a pillanatnyi $r$-t, $v$-t és $dv/dt$-t, az $a_{cp}$ és $a_t$ összetevők ugyanúgy kiszámíthatók, mint körmozgásnál.
- Általános esetben ezek az összetevők **folyamatosan változnak** (nagyságuk és irányuk is), de adott pillanatban egyszerűen számolhatók.

---

### 2.2 Képletek

| Képlet | Jelek | Mértékegység |
|---|---|---|
| $\theta = \dfrac{s}{r}$ (4-1) | $\theta$: szögkoordináta; $s$: a körív hossza; $r$: a kör sugara | rad (dimenzió nélküli); m; m |
| $1\ \text{rad} = \dfrac{360^\circ}{2\pi}\approx57{,}3^\circ$ | | |
| $v = \dfrac{2\pi r}{T}$ | egy fordulat alatt megtett út ($2\pi r$) osztva a periódusidővel; $v$: sebesség nagysága; $T$: periódusidő | m/s; s |
| $a_t = \dfrac{dv}{dt}$ (4-2) | tangenciális (érintő menti) gyorsulás | m/s² |
| $a_{cp} = \dfrac{v^2}{r}$ (4-8) | centripetális gyorsulás (sugár irányban **befelé**) | m/s² |
| $a_{cp} = \dfrac{4\pi^2 r}{T^2}$ | a $v = 2\pi r/T$ behelyettesítésével | m/s² |
| $a = \sqrt{a_t^2 + a_{cp}^2}$ | az eredő (teljes) gyorsulás nagysága | m/s² |
| $\operatorname{tg}\varphi = \dfrac{a_{cp}}{a_t}$ | $\varphi$: az eredő gyorsulás és a **mozgás iránya (érintő)** közötti szög | ° |
| $\mathbf a = -\dfrac{v^2}{r}\,\hat{\mathbf r} + \dfrac{dv}{dt}\,\hat{\boldsymbol\theta}$ (4-9) | teljes gyorsulás vektoros alakban; $\hat{\mathbf r}$: kifelé, $\hat{\boldsymbol\theta}$: érintő irányú egységvektor | m/s² |

A **dimenzió-ellenőrzés** ($v^2/r$ gyorsulás-dimenziójú): $\dfrac{[L/T]^2}{[L]} = \dfrac{L}{T^2}$ ✔

**Kiegészítés** (a fejezet szövege nem definiálja külön, de a fejezet végi feladatok használják: fordulatszám, szöggyorsulás). A körmozgás szokásos mennyiségei:

| Mennyiség | Képlet | Mértékegység |
|---|---|---|
| Frekvencia (fordulatszám) | $f = \dfrac{1}{T}$ | 1/s = Hz (percenkénti fordulat: osztás 60-nal) |
| Szögsebesség | $\omega = \dfrac{\Delta\theta}{\Delta t} = \dfrac{d\theta}{dt} = \dfrac{2\pi}{T} = 2\pi f$ | rad/s |
| Kerületi sebesség | $v = \omega\, r$ | m/s |
| Centripetális gyorsulás | $a_{cp} = \omega^2 r = v\,\omega$ | m/s² |
| Szöggyorsulás | $\alpha = \dfrac{d\omega}{dt}$ | rad/s² |
| Tangenciális gyorsulás | $a_t = \alpha\, r$ | m/s² |

- Levezetés: $\theta = s/r \Rightarrow s = r\theta$, deriválva $v = \dfrac{ds}{dt} = r\dfrac{d\theta}{dt} = r\omega$; ebből $a_{cp} = v^2/r = \omega^2 r$ és $a_t = \dfrac{dv}{dt} = r\dfrac{d\omega}{dt} = r\alpha$.

#### Diákmankó (háromszögek)

Takard le a keresettet! Egymás mellett: szorzás, egymás felett: osztás.

```
     ív, szög, sugár              centripetális gyorsulás           kerületi sebesség (kiegészítés)

          /\                            /\                                /\
         /  \                          /  \                              /  \
        / s  \                        / v² \                            / v  \
       /------\                      /------\                          /------\
      / θ | r  \                    / a | r  \                        / ω | r  \
     /__________\                  /__________\                      /__________\

  s = θ · r   θ = s / r         v² = a · r    a = v² / r          v = ω · r   ω = v / r
  r = s / θ                     r = v² / a                         r = v / ω
```

- Az eredő gyorsulás: **két merőleges összetevő → Pitagorasz**: $a = \sqrt{a_t^2 + a_{cp}^2}$, a szög: $\operatorname{tg}\varphi = a_{cp}/a_t$.
- **Fordulat/perc → periódusidő:** pl. 33,3 fordulat/perc: $T = \dfrac{1\ \text{perc}}{33{,}3}\cdot\dfrac{60\ \text{s}}{1\ \text{perc}} = 1{,}80\ \text{s}$.

#### Levezetések

**(a) $\theta = s/r$ és a radián:** a definíció szerint a szög radiánban az ív és a sugár hányadosa. Ha $s = r$, akkor $\theta = 1$ rad. A teljes körívre $s = 2\pi r$, így $\theta = 2\pi$ rad $= 360^\circ$.

**(b) A centripetális gyorsulás levezetése (egyenletes körmozgás):**

1. A sebességváltozás: $\Delta\mathbf v = \mathbf v(t+\Delta t) - \mathbf v(t)$, tehát $\mathbf v(t) + \Delta\mathbf v = \mathbf v(t+\Delta t)$ (4-3, 4-4).
2. A két sebességvektor közti szög $\Delta\theta$ **ugyanakkora**, mint a két helyvektor ($\mathbf r(t)$, $\mathbf r(t+\Delta t)$) közti szög, mert a sebességvektor mindig **merőleges** a sugárra (érintő). Ha a helyvektor $\Delta\theta$ szöggel elfordul, a sebességvektornak is pontosan ennyivel kell elfordulnia.
3. A két (egyenlő szárú) háromszög (sebességvektorok: $v, v, \Delta v$; helyvektorok: $r, r, \Delta r$) **hasonló**, mert ugyanaz a csúcsszögük ($\Delta\theta$). Ezért (4-5):
   $$\frac{\Delta v}{v} = \frac{\Delta r}{r} \approx \frac{\Delta s}{r}$$
   (kis $\Delta\theta$-nál az $\Delta s$ ívhossz jól közelíthető a $\Delta r$ húrral).
4. Átrendezve (4-6): $\Delta v \approx \left(\dfrac{v}{r}\right)\Delta s$.
5. A gyorsulás definíciójába helyettesítve ($v/r$ állandó, ezért kiemelhető) (4-7):
   $$a_{cp} = \lim_{\Delta t\to0}\frac{\Delta v}{\Delta t} = \frac{v}{r}\lim_{\Delta t\to0}\frac{\Delta s}{\Delta t}$$
6. A határértékben a közelítés egyenlőséggé válik, és $\lim \Delta s/\Delta t$ a pálya menti pillanatnyi sebesség, tehát $v$:
   $$\boxed{a_{cp} = \frac{v^2}{r}}\quad\text{(4-8)}$$
7. **Irány:** $\Delta\theta\to0$ esetén $\Delta\mathbf v$ **radiálisan befelé** mutat és **merőleges** $\mathbf v$-re. Így a gyorsulás a kör középpontja felé irányul (4-4 ábra).

**(c) $a_{cp} = 4\pi^2 r/T^2$:** egy fordulat alatt a test $2\pi r$ utat tesz meg $T$ idő alatt, ezért $v = 2\pi r/T$. Behelyettesítve: $a_{cp} = \dfrac{(2\pi r/T)^2}{r} = \dfrac{4\pi^2 r}{T^2}$.

**(d) A gyorsulás két összetevője:** a sebességvektor $\mathbf v = v\,\hat{\boldsymbol\theta}$. Deriválva idő szerint két tag adódik: a nagyság változása ($\dfrac{dv}{dt}\hat{\boldsymbol\theta}$) és az irány változása (ez adja a sugár irányú, befelé mutató $-\dfrac{v^2}{r}\hat{\mathbf r}$ tagot). Ezért a (4-9) összefüggés.

---

### 2.3 Feladatok levezetése (a fejezet példái)

#### 4-1 példa: lemezjátszó korongja
*Mekkora a gyorsulása annak a részecskének, amely egy lemezjátszó állandó, percenként 33,3 fordulatszámmal forgó korongján a középponttól 12 cm-re helyezkedik el?*

- A korong állandó sebességgel forog → csak **centripetális** gyorsulás van: $a_{cp} = \dfrac{v^2}{r}$.
- **Periódusidő:** $T = \dfrac{1\ \text{perc}}{33{,}3}\cdot\dfrac{60\ \text{s}}{1\ \text{perc}} = 1{,}80\ \text{s}$
- **Sebesség:** $v = \dfrac{\text{egy fordulat alatt megtett út}}{\text{egy fordulathoz szükséges idő}} = \dfrac{2\pi r}{T} = \dfrac{2\pi\cdot0{,}12}{1{,}80} = 0{,}419\ \text{m/s}$
- **Gyorsulás:**
  $$a_{cp} = \frac{v^2}{r} = \frac{4\pi^2 r}{T^2} = \frac{4\pi^2\cdot0{,}12\ \text{m}}{(1{,}80\ \text{s})^2} = \boxed{1{,}46\ \text{m/s}^2}$$
- **Tanulság:** a részecske a kör középpontja felé gyorsul, bár a sebessége (az érintő irányában) a kör érintőjébe mutat. Görbe pályán mozgó test gyorsulásvektora sosem azonos irányú a sebességvektorral. Az $a_{cp}$ irányát a $\mathbf v$ **irányának változása** szabja meg.

#### 4-2 példa: gyorsuló autó körpályán
*Egy gépkocsi 20 m sugarú körpályán mozog, és a sebességét másodpercenként 0,6 m/s-mal növeli. Határozzuk meg a gyorsulás a) tangenciális, b) centripetális komponensét, c) a teljes gyorsulás nagyságát és irányát abban az időpontban, amikor a pillanatnyi sebesség 4 m/s.*

- **a)** A tangenciális gyorsulás csak a sebesség megváltozásának mértékétől függ:
  $$a_t = 0{,}600\ \text{m/s}^2$$
- **b)** A centripetális összetevő a sugártól és a **pillanatnyi** sebességtől függ:
  $$a_{cp} = \frac{v^2}{r} = \frac{(4\ \text{m/s})^2}{20\ \text{m}} = 0{,}800\ \text{m/s}^2$$
- **c)** Eredő gyorsulás (két merőleges összetevő, Pitagorasz):
  $$a = \sqrt{a_t^2 + a_{cp}^2} = \sqrt{0{,}600^2 + 0{,}800^2} = \boxed{1{,}00\ \text{m/s}^2}$$
- **Irány:** a mozgás irányával (érintővel) bezárt szög:
  $$\varphi = \operatorname{arc\,tg}\frac{a_{cp}}{a_t} = \operatorname{arc\,tg}\frac{0{,}800}{0{,}600} = \boxed{53{,}1^\circ}$$
- Mivel a sebesség **nő**, $a_t$ a mozgás irányába mutat. $a_{cp}$ befelé. Az eredő a kettő közé esik.

#### 4-3 példa: gyorsulás kifejezése $\hat{\mathbf r}$ és $\hat{\boldsymbol\theta}$ egységvektorokkal
*Fejezzük ki egy gépkocsi gyorsulását az $\hat{\boldsymbol\theta}$ és $\hat{\mathbf r}$ egységvektorok segítségével.*

- Feltéve, hogy a gépkocsi a pozitív $\hat{\boldsymbol\theta}$ irányban mozog és **lassul**, a gyorsulás érintő irányú komponense **negatív**:
  $$\mathbf a = -\left(1{,}39\ \tfrac{\text{m}}{\text{s}^2}\right)\hat{\boldsymbol\theta} - \left(2{,}78\ \tfrac{\text{m}}{\text{s}^2}\right)\hat{\mathbf r}$$
- Mindkét tag negatív: az érintő menti tag azért, mert lassul, a sugár irányú tag azért, mert a centripetális gyorsulás befelé mutat ($\hat{\mathbf r}$ kifelé).

> ⚠️ **Eltérés a könyvben (ellenőrizd a nyomtatott könyvben!):** a példa szövege szerint „az előző feladatban leírt gépkocsi" gyorsulását kell kifejezni, de a megadott számok (1,39 és 2,78 m/s²) a **4-4 példa** autójához tartoznak (lassító autó, görbületi sugár 100 m, 60 km/h). A 4-2 példa gyorsuló autójára (0,600 és 0,800 m/s²) a felírás ez lenne: $\mathbf a = (0{,}600\ \text{m/s}^2)\,\hat{\boldsymbol\theta} - (0{,}800\ \text{m/s}^2)\,\hat{\mathbf r}$, hiszen ott a sebesség nő (az érintő menti tag pozitív).
> A PDF-ben két-három helyen a $\theta$-s szimbólum helyén „Error! Objects cannot be created…" felirat látszik. Ezek $\hat{\boldsymbol\theta}$ és $\Delta\theta$ szimbólumok, a jelentésük egyértelmű.

#### 4-4 példa: lassító autó görbe úton (általános görbe vonalú mozgás)
*Egy gépkocsi görbe vonalú úton halad. Amint egy 100 m görbületi sugarú szakaszra ér, a vezető másodpercenként 5 km/órával csökkenti a sebességét. Mekkora a gépkocsi gyorsulása abban a pillanatban, amikor 60 km/óra sebességgel mozog?*

- **Tangenciális összetevő** (átváltás: km/h → m/s):
  $$a_t = \frac{5\ \text{km/h}}{1\ \text{s}} = 5\cdot\frac{1000\ \text{m}}{3600\ \text{s}}\cdot\frac{1}{1\ \text{s}} = 1{,}39\ \text{m/s}^2$$
  Mivel az autó **lassul**, ez az összetevő a mozgás irányával **ellentétes**.
- **Centripetális összetevő:** először a sebesség m/s-ban:
  $$v = 60\cdot\frac{1000}{3600} = 16{,}7\ \text{m/s}\quad\Rightarrow\quad a_{cp} = \frac{v^2}{r} = \frac{(16{,}7)^2}{100} = 2{,}78\ \text{m/s}^2$$
  Ez merőleges a pályára, a pillanatnyi görbületi középpont felé mutat.
- **Teljes gyorsulás nagysága:**
  $$a = \sqrt{1{,}39^2 + 2{,}78^2} = \boxed{3{,}11\ \text{m/s}^2}$$
- **Irány:** a pálya érintőjétől mért szög:
  $$\varphi = \operatorname{arc\,tg}\frac{a_{cp}}{a_t} = \operatorname{arc\,tg}\frac{2{,}78}{1{,}39} = \boxed{63{,}4^\circ}$$
  (a 4-8b ábrán látható módon).

---

### 2.4 Egyszerű módja a téma megértésének

**Gondolj egy zsinóron pörgetett labdára:**
- A labda sebessége **mindig** a kör érintője mentén mutat (ha elengeded a zsinórt, a labda ebbe az irányba repül tovább).
- A zsinór **befelé húzza** a labdát. A labda így **folyamatosan befelé „esik"** (befelé gyorsul), de a sebessége miatt közben oldalirányban halad, ezért sosem ér a középpontba, hanem körben marad.

**Alapgondolat:**
> *A gyorsulás nem azt jelenti, hogy gyorsabb leszel, hanem azt, hogy **változik a sebességvektor**: akár a nagysága, akár az iránya.*

Ezért egy állandó sebességgel kanyarodó autóban is gyorsulsz (érzed, hogy oldalra „taszít").

**Két összetevő, két feladat:**
- **Érintő menti gyorsulás ($a_t$):** „Mennyivel változik a *sebességmérő* állása?" → a sebesség **nagyságának** változása. Az érintő irányába mutat.
- **Sugár irányú (centripetális) gyorsulás ($a_{cp}$):** „Mennyire kanyarodik a test?" → a sebesség **irányának** változása. Mindig befelé mutat. $a_{cp} = v^2/r$.
- A kettő **merőleges** egymásra → Pitagorasz.

**Mit mutat a képlet?** $a_{cp} = v^2/r$:
- **Nagyobb sebességnél** nagyobb a centripetális gyorsulás, és négyzetesen nő (kétszeres sebesség → négyszeres gyorsulás).
- **Kisebb sugárnál** (szűkebb kanyar) nagyobb a gyorsulás.

**Feladatmegoldási recept:**
1. **Vázlat:** rajzold fel a kört, a test helyzetét, az érintőt (sebesség iránya) és a sugarat (a középpont felé).
2. **Mértékegységek:** fordulat/perc → fordulat/s, km/h → m/s, fokok → radián.
3. Ha kell: $T$ vagy $f$ → $v = 2\pi r/T$.
4. $a_{cp} = v^2/r$ (mindig a középpont felé).
5. Ha a sebesség nagysága is változik: $a_t = dv/dt$, majd $a = \sqrt{a_t^2 + a_{cp}^2}$ és $\operatorname{tg}\varphi = a_{cp}/a_t$ (a szöget az **érintőtől** mérjük).
6. **Ellenőrzés:** a gyorsulás dimenziója m/s², a szögfüggvény argumentuma radián/fok a számológép beállításának megfelelően.

**Gyakori hibák:**
- „Állandó sebességű körmozgásnál nincs gyorsulás." → **Rossz!** A sebességvektor iránya változik, ezért van gyorsulás ($v^2/r$).
- **Centripetális ≠ centrifugális:** a centripetális gyorsulás **befelé**, a centrifugális **kifelé** mutat.
- A sebességnagyság állandósága **nem** jelenti a sebességvektor állandóságát.
- Az $a_{cp}$ és $a_t$ nem azonos mennyiség: $a_t$ csak a sebesség **nagyságának** változását írja le.
- A szögeket **radiánban** kell használni a kinematikai egyenletekben ($\theta = s/r$).
- Az $a_{cp}$ **iránya változik** a mozgás közben (mindig a középpont felé mutat), csak a nagysága állandó egyenletes körmozgásnál.
- Gyorsulásnál ne felejtsd el, hogy a lassuló autó $a_t$ komponense a mozgással **ellentétes**.

---

## 3. Téma lezárása

### Rövid emlékeztető: mit tanultunk?
- **Polárkoordináták:** $(r,\theta)$; körmozgásnál $r$ állandó. $\theta = s/r$ **radiánban** ($2\pi$ rad $= 360^\circ$, $1$ rad $\approx 57{,}3^\circ$).
- A körmozgás **sebessége mindig érintő irányú**.
- **Egyenletes körmozgás:** a sebességnagyság állandó, de a **gyorsulás nem nulla**: $a_{cp} = v^2/r = 4\pi^2 r/T^2$, **a kör középpontja felé** mutat, és **merőleges** a sebességre.
- **Nem egyenletes körmozgás:** $a_t = dv/dt$ (érintő irányú) **és** $a_{cp} = v^2/r$ (befelé); eredőjük $a = \sqrt{a_t^2 + a_{cp}^2}$, iránya $\operatorname{tg}\varphi = a_{cp}/a_t$.
- Vektoros alak: $\mathbf a = -\dfrac{v^2}{r}\hat{\mathbf r} + \dfrac{dv}{dt}\hat{\boldsymbol\theta}$.
- **Általános görbe vonalú mozgás:** minden pontban van **görbületi kör** (görbületi sugár és középpont). Az $a_{cp}$ és $a_t$ ugyanúgy számolható.
- **Fontos megkülönböztetés:** centripetális (befelé) és centrifugális (kifelé).

### Rövid befejezés
A körmozgás megmutatta, hogy a gyorsulás fogalma sokkal tágabb, mint „gyorsabban megyek": a sebességvektor bármilyen megváltozása gyorsulás. Ezzel a kinematika (a mozgás leírása) teljessé vált: tudjuk, hogy **hogyan** mozog egy test egyenes vonalon, síkban, térben és körpályán. Egy kérdés maradt nyitva: **miért** gyorsul egy test? Például mi tartja körpályán a zsinóron pörgetett labdát, vagy mi gyorsítja a Hold felé a Holdat?

### Gyakorló feladatok a fejezet végén (a könyvből)
| Alfejezet | Feladatok |
|---|---|
| 4.2 Polárkoordináták | 4A-1 … 4B-3 |
| 4.3–4.4 Körmozgás, általános görbe vonalú mozgás | 4A-4 … 4B-22 |
| További feladatok | 4C-23 … 4C-28 |

- A **kérdések (1–7)** fogalmi gyakorlásra valók (pl. gyorsul-e az az autó, amelynek a sebessége állandó; lehet-e a sebesség nulla és a gyorsulás nem; mit jelent a „g-többszörös" gyorsulás; milyen irányú lehet az eredő gyorsulás görbe pályán).
- Az **utolsó feladatok** (4C-23…) az előző fejezetek (pl. hajítás) tudásával is összekapcsolják a körmozgást (pl. műholdak pályája, elszakadó fonal).
- A **páratlan sorszámú feladatok** megoldása a könyv végén található (IV. fejezet, A-18 oldal).

### ➡️ Következő modul
**Newton-féle mozgástörvények:** [[newton_fele_mozgastorvenyek]]
