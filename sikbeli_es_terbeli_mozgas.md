# Síkbeli és térbeli mozgás

> Forrás: a könyv III. fejezete (3.1–3.7 + Összefoglalás, Kérdések, Feladatok).
> Ez a modul az előző (egyenesvonalú mozgások) általánosítása: ugyanazok a fogalmak (hely, sebesség, gyorsulás), csak **vektorként** két és három dimenzióban.

---

## 1. Téma bevezetése

### Mi a téma?
Pontszerű részecske mozgásának leírása **síkban (2D)** és **térben (3D)**. Eszköze a **vektor**. A fejezet végén a legfontosabb alkalmazás: a **hajítások** (vízszintes és ferde hajítás).

### Mi a téma jelentése?
- Az előző fejezetben a mozgás egyenes mentén zajlott, ott elég volt a mennyiségek előjele (+/−) az irány jelzésére. Síkban és térben már **nagyság és irány** is kell. Erre valók a **vektorok**.
- Az általános térbeli mozgás legtöbb alapvető tulajdonsága már **kétdimenziós** mozgásnál is megjelenik, ezért többnyire síkbeli mozgásokkal foglalkozunk.
- A három mennyiség, amelynek nagysága és iránya is van: az **elmozdulás** ($\Delta\mathbf r$), a **sebesség** ($\mathbf v$) és a **gyorsulás** ($\mathbf a$).
- **Nagy felismerés (Galilei):** a mozgás vízszintes és függőleges összetevője **egymástól független**. Így egy bonyolult kétdimenziós pálya két egyszerű egydimenziós mozgásra bontható, amit az előző fejezetből már tudunk.

### Mindennapi előfordulás, felhasználás
- **Mindennapokban:** eldobott labda, kirúgott focilabda, ugrás, kidobott kő, vízsugár ívelése, autó útja két város között, hajó vagy repülő útvonala (irány + távolság), helikopter, térkép- és navigációs adatok.
- **Fizikában:**
  - **vektorok** minden későbbi témában (erők, impulzus, mezők),
  - **hajítások, lövedékek** pályája,
  - a fizikai törvények **vektoros alakja** független a koordinátarendszer választásától (ez mély tulajdonság, lásd lent: invariancia),
  - gömbi, hengeres koordináták: földrajzi szélesség/hosszúság, csillagászat.

---

## 2. Téma kifejtése

### 2.1 Alapfogalmak

#### Skalár és vektor
- **Skalár:** csak nagysága van (pl. idő, tömeg, hőmérséklet, terület, szín).
- **Vektor:** **nagysága és iránya** is van. Geometriailag **irányított szakasz**, a nyílhegy az irányt, a szakasz hossza a nagyságot mutatja.
- Jelölés: nyomtatásban **félkövér betű** ($\mathbf r$), kézírásban a betű fölé húzott kis nyíl ($\vec r$). A **nagyságot (abszolút értéket)** $|\mathbf r|$ vagy egyszerűen $r$ jelöli.
- A fizikai mennyiséget ábrázoló vektornak mindig van **dimenziója/mértékegysége** (pl. a helyvektoré méter).

#### Kétdimenziós koordinátarendszerek (3-1 ábra)
- **Derékszögű (Descartes) koordináták $(x,\,y)$:** a pontból a tengelyekre bocsátott merőlegesek a tengelyekből kimetszik az $x$ és $y$ koordinátát.
- **Síkbeli polárkoordináták $(r,\,\theta)$:**
  - $r$ = az origót a ponttal összekötő szakasz hossza,
  - $\theta$ = az origót a ponttal összekötő egyenes szöge a **pozitív $x$ tengellyel**, az **óramutató járásával ellentétes** irányban mérve.

#### Helyzetvektor ($\mathbf r$)
- Az origótól az adott $P$ ponthoz mutató vektor. Megadja a pont helyét az origóhoz képest.
- **Komponensek (összetevők):** a vektor végpontjából a tengelyekre bocsátott merőlegesek éppen a $P$ pont koordinátáit metszik ki. Az összetevők lehetnek **pozitívak vagy negatívak**, attól függően, hogy a komponens az origótól milyen irányba mutat.
- **Komponensekre bontás:** a vektor meghatározása az összetevőivel. A komponensek egyértelműen megadják a vektort.

#### Műveletek skalárral
- Vektor × szám: a vektor nagysága a szám abszolút értékével szorzódik. Pl. $2\mathbf A$ kétszer olyan hosszú, $\tfrac12\mathbf A$ fele akkora.
- **Szorzás −1-gyel:** az **ellentett (negatív)** vektort kapjuk, azonos nagyság, **ellentétes irány** ($\mathbf A$ és $-\mathbf A$ antiparalel).
- Osztani skalárral nem kell külön definiálni, mert az az egynél kisebb számmal való szorzás.

#### Egységvektorok
- $\hat{\mathbf x}$, $\hat{\mathbf y}$, $\hat{\mathbf z}$: **egységnyi hosszúságú** vektorok, amelyek a megfelelő tengely **pozitív irányába** mutatnak. **Dimenziójuk nincs**, csak az irányt jelzik.
- Egy tetszőleges vektor felírható **komponensekkel**: $\mathbf C = C_x\,\hat{\mathbf x} + C_y\,\hat{\mathbf y}$ (3D-ben + $C_z\,\hat{\mathbf z}$).
- Más jelölések: $\hat{\mathbf i}, \hat{\mathbf j}, \hat{\mathbf k}$ (ezt gyakran használják az iskolában). Ugyanazt jelentik.
- Skalár × egységvektor = vektor, amelynek nagysága a skalár értéke, iránya az egységvektoré.

#### Elmozdulásvektor ($\Delta\mathbf r$)
- A **kezdő- és végpont közti** vektor: $\Delta\mathbf r = \mathbf r_2 - \mathbf r_1$.
- **Nagysága nem az úthossz**, hanem a két pont közötti **legrövidebb (egyenes) szakasz** hossza, a pálya tényleges alakjától függetlenül.

#### Vektorok összeadása és kivonása
- **Összeadás geometriailag:** a vektorokat (nagyság és irány megtartásával) eltolhatjuk. Az egyik vektor végpontjából mérjük fel a másikat. Az **összeg** az első kezdőpontjából a második végpontjába mutató vektor.
  - **Kommutatív:** $\mathbf A + \mathbf B = \mathbf B + \mathbf A$
  - **Asszociatív:** $(\mathbf A + \mathbf B) + \mathbf C = \mathbf A + (\mathbf B + \mathbf C)$
  - Kettőnél több vektor: **sokszögmódszer** (egymás után fűzzük a nyilakat, az összeg az első kezdőpontjából az utolsó végpontjába mutat).
- **Kivonás:** $\mathbf D = \mathbf A - \mathbf B = \mathbf A + (-\mathbf B)$, vagyis az ellentettet adjuk hozzá. **Nem cserélhető fel:** $\mathbf A - \mathbf B = -(\mathbf B - \mathbf A)$.
- Két vektor **különbségének** abszolút értéke **lehet nagyobb**, mint az **összegüké** (ha pl. nagyjából ellentétes irányba mutatnak).
- **Algebrai módszer (pontos):** a komponenseket külön-külön adjuk össze, illetve vonjuk ki.

> ⚠️ **Előjel-figyelmeztetés a vektorábrákon:** negatív előjelet vektordiagramon **csak akkor** használj, ha egy másik, szintén szereplő vektor **ellentettjét** akarod jelölni. Soha ne írj negatív előjelet egy vektorhoz csak azért, mert az történetesen negatív koordináta felé mutat. (Pl. a lefelé mutató nehézségi gyorsulást ne jelöld $-\mathbf g$-vel, hanem a nagyságot $g$-vel, az irányt az ábra mutatja.) A negatív előjel félreértéshez vezethet, mert azt sugallja, hogy az „igazi" vektor az ellenkező irányba mutat.

#### Térbeli (3D) koordinátarendszerek és jobbrendszer
- **Descartes-féle térbeli rendszer:** három, egymásra merőleges tengely: $x$, $y$, $z$.
- A $z$ tengely irányítása kétféle lehet. A megállapodás szerint **jobbrendszert** használunk:
  - **Jobbkéz-szabály:** a jobb kéz hüvelykujját kifeszítve, a többi ujjat az $x$ pozitív iránya felől az $y$ pozitív iránya felé hajlítjuk. A hüvelykujj mutatja a **$z$ pozitív irányát**.
  - Más szavakkal: egy jobbmenetes csavar, amit az $x$-ből $y$-ba forgatunk, a $z$ irányába halad.
- Térbeli vektor: $\mathbf B = B_x\hat{\mathbf x} + B_y\hat{\mathbf y} + B_z\hat{\mathbf z}$.
- **Más térbeli koordinátarendszerek** (3-17 ábra): hengerkoordináták $(\rho,\varphi,z)$, gömbi polárkoordináták $(r,\theta,\varphi)$. Mindegyik **három** paramétert használ a helyzet megadására. A Földön a helyzetet két szög adja meg: **hosszúsági szög** (a Greenwichen átmenő kezdő hosszúsági körtől keletre/nyugatra) és **szélességi szög** (az egyenlítőtől északra/délre).

#### Sebesség és gyorsulás vektorként
- **Átlagsebesség-vektor:** az elmozdulásvektor és az eltelt idő hányadosa.
- **Pillanatnyi sebesség ($\mathbf v$):** az átlagsebesség-vektor határértéke, amikor $\Delta t\to0$ (a helyvektor idő szerinti deriváltja). **Mindig a pálya érintőjébe esik és a haladás irányába mutat** (mert $\Delta t\to0$-nál $\Delta\mathbf r$ iránya az érintő irányához közelít).
- **Átlagos gyorsulás:** a sebességvektor megváltozása ($\Delta\mathbf v$, két vektor **különbsége**) osztva az idővel.
- **Pillanatnyi gyorsulás ($\mathbf a$):** az átlagos gyorsulás határértéke, a sebességvektor idő szerinti deriváltja.
- **Fontos:** a sebesség- és gyorsulásvektor lehet **nagyságában ÉS irányában** is változó. Az $\mathbf r$, $\mathbf v$, $\mathbf a$ vektorok **iránya nem szükségképpen azonos**. (Példa: eldobott labdánál $\mathbf v$ a pálya érintője, $\mathbf a$ mindig lefelé mutat, $\mathbf r$ az origóból a labdához mutat.)
- A pálya csúcspontján a pillanatnyi sebesség **függőleges összetevője nulla**, de a gyorsulás ugyanúgy $g$, lefelé. (Függőlegesen feldobott testnél a csúcson a **teljes** sebesség nulla, a gyorsulás még mindig $g$ lefelé.)

#### Invariancia (miért jó a vektorjelölés?)
- A fizikai törvények **vektoros alakja ugyanaz marad**, ha a koordinátarendszert **eltoljuk** (az origó helye változik, a tengelyek párhuzamosak maradnak), vagy **elforgatjuk**. Ezt hívják **invarianciának**.
- Ezért a vektoros egyenletek **bármely, tetszőlegesen választott koordinátarendszerben érvényesek**, és a számolás nagy részét megkönnyítik.

#### Hajítások: alapgondolat
- Kis magasságkülönbségnél és ha a légellenállás elhanyagolható, a gravitációs gyorsulás **állandó**: $g = 9{,}81\ \text{m/s}^2$ (nagysága), iránya **lefelé**. Minden szabadon eső test ugyanakkora gyorsulással esik.
- **Galilei felfedezése:** a szabadon eső (hajított) testek mozgásának **vízszintes és függőleges összetevője teljesen független egymástól**.
  - Szemléltetés (3-26 ábra, villanófényes felvétel): az egyik golflabdát leejtik, a másikat egyszerre **vízszintesen elhajítják** (2 m/s). A két labda **ugyanabban az ütemben süllyed**. A vízszintes sebesség a függőleges mozgásra nincs hatással.
- A pálya egy **parabola** (3C-37 feladat).
- A függetlenség **csak** állandó $g$ és elhanyagolható légellenállás mellett igaz (más esetekben pl. körmozgásnál, Coriolis-erőnél az összetevők összefüggenek, ezek későbbi fejezetek).

---

### 2.2 Képletek

#### Koordináták, polár ↔ derékszögű (3-1)

| Képlet | Jelek | Mértékegység |
|---|---|---|
| $x = r\cos\theta$ | $x$: x-koordináta; $r$: a vektor nagysága; $\theta$: a +x tengelytől **ellentétes óramutató** irányban mért szög | m; m; ° vagy rad |
| $y = r\sin\theta$ | $y$: y-koordináta | m |
| $r = \sqrt{x^2 + y^2}$ | (Pitagorasz-tétel) | m |
| $\operatorname{tg}\theta = \dfrac{y}{x}$ | $\theta = \operatorname{arc\,tg}(y/x)$ **a megfelelő negyedben** | – |

**Negyed-szabály (nagyon fontos!):** a számológép az $\operatorname{arc\,tg}$-t csak $-90^\circ\ldots+90^\circ$ között adja. Ezért **mindig rajzolj vázlatot**, és számold ki a **hegyesszöget** $\varphi = \operatorname{arc\,tg}\left|\dfrac{y}{x}\right|$ az **$x$ tengellyel**, majd:

| Hol van a vektor? | $\theta$ (a +x tengelytől, ellentétes óramutató irányban) |
|---|---|
| I. negyed ($x>0,\ y>0$) | $\theta = \varphi$ |
| II. negyed ($x<0,\ y>0$) | $\theta = 180^\circ - \varphi$ |
| III. negyed ($x<0,\ y<0$) | $\theta = 180^\circ + \varphi$ |
| IV. negyed ($x>0,\ y<0$) | $\theta = 360^\circ - \varphi$ |

(A fejezet példáiban pontosan ez történik: lásd 3-3 és 3-4 példa.)

#### Vektorok és komponensek

| Képlet | Jelek | Mértékegység |
|---|---|---|
| $\mathbf r = x\hat{\mathbf x} + y\hat{\mathbf y} + z\hat{\mathbf z}$ | $\mathbf r$: helyzetvektor; $x,y,z$: komponensei | m |
| $\lvert\mathbf r\rvert = \sqrt{x^2 + y^2 + z^2}$ | nagyság | m |
| $\Delta\mathbf r = \mathbf r_2 - \mathbf r_1$ | elmozdulásvektor; $\mathbf r_1$: kezdeti, $\mathbf r_2$: végső helyzetvektor | m |
| $\Delta r_x = x_2 - x_1,\ \Delta r_y = y_2 - y_1$ | komponensek: végső − kezdeti | m |
| $\mathbf C = \mathbf A + \mathbf B \Rightarrow C_x = A_x + B_x,\ C_y = A_y + B_y$ | összeadás komponensenként | (a vektor mértékegysége) |
| $\mathbf D = \mathbf A - \mathbf B \Rightarrow D_x = A_x - B_x,\ D_y = A_y - B_y$ | kivonás komponensenként | (a vektor mértékegysége) |
| $\lvert\mathbf C\rvert = \sqrt{C_x^2 + C_y^2}$ | az eredő nagysága | |

#### Sebesség és gyorsulás

| Képlet | Jelek | Mértékegység |
|---|---|---|
| $\mathbf v_{\text{átl}} = \dfrac{\Delta\mathbf r}{\Delta t}$ (3-4) | átlagsebesség-vektor | m/s |
| $\mathbf v = \lim\limits_{\Delta t\to0}\dfrac{\Delta\mathbf r}{\Delta t} = \dfrac{d\mathbf r}{dt}$ (3-5) | pillanatnyi sebességvektor | m/s |
| $\mathbf v = v_x\hat{\mathbf x} + v_y\hat{\mathbf y} + v_z\hat{\mathbf z}$ (3-6) | | m/s |
| $v_x = \dfrac{dx}{dt},\ v_y = \dfrac{dy}{dt},\ v_z = \dfrac{dz}{dt}$ (3-7) | a sebesség komponensei = a koordináták deriváltjai | m/s |
| $\lvert\mathbf v\rvert = \sqrt{v_x^2 + v_y^2 + v_z^2}$ | a sebesség nagysága | m/s |
| $\mathbf a_{\text{átl}} = \dfrac{\Delta\mathbf v}{\Delta t}$ (3-8) | átlagos gyorsulás; $\Delta\mathbf v = \mathbf v(t+\Delta t) - \mathbf v(t)$ | m/s² |
| $\mathbf a = \lim\limits_{\Delta t\to0}\dfrac{\Delta\mathbf v}{\Delta t} = \dfrac{d\mathbf v}{dt}$ (3-9) | pillanatnyi gyorsulásvektor | m/s² |
| $a_x = \dfrac{dv_x}{dt},\ a_y = \dfrac{dv_y}{dt},\ a_z = \dfrac{dv_z}{dt}$ (3-11) | a gyorsulás komponensei | m/s² |

**Állandó gyorsulás esetén** ugyanazok az egyenletek, mint az egyenesvonalú mozgásnál, **komponensenként külön-külön** felírva (a $t$ ugyanaz mindenütt!):

$$v_x = (v_x)_0 + a_x t \qquad v_y = (v_y)_0 + a_y t \qquad v_z = (v_z)_0 + a_z t$$
$$x = x_0 + (v_x)_0\,t + \tfrac12 a_x t^2 \qquad \text{(és hasonlóan } y,\ z\text{)}$$

#### Hajítás (felfelé pozitív $y$, $a_x = 0$, $a_y = -g$)

Legyen a kezdősebesség $v_0$, a **vízszintessel bezárt szög** $\theta_0$.

| Képlet | Jelentés | Mértékegység |
|---|---|---|
| $(v_x)_0 = v_0\cos\theta_0$ | kezdősebesség vízszintes összetevője | m/s |
| $(v_y)_0 = v_0\sin\theta_0$ | kezdősebesség függőleges összetevője | m/s |
| $v_x = v_0\cos\theta_0$ (állandó!) | vízszintes sebesség | m/s |
| $v_y = v_0\sin\theta_0 - g\,t$ | függőleges sebesség | m/s |
| $x = x_0 + v_0\cos\theta_0\cdot t$ | vízszintes helyzet | m |
| $y = y_0 + v_0\sin\theta_0\cdot t - \tfrac12 g t^2$ | függőleges helyzet | m |
| $\lvert\mathbf v\rvert = \sqrt{v_x^2 + v_y^2}$ | pillanatnyi sebesség nagysága | m/s |
| $\operatorname{tg}\varphi = \dfrac{\lvert v_y\rvert}{\lvert v_x\rvert}$ | a sebességvektor szöge a vízszintessel | – |

**Jelek:** $g = 9{,}81\ \text{m/s}^2$ (pozitív szám!), $t$ az idő (s), $x_0, y_0$ a kezdeti helyzet (m).
Ha a **lefelé** irányt választod pozitívnak, akkor $a_y = +g$ és a lefelé mutató komponensek pozitívak (lásd 3-9 példa).

**Kiegészítés (a fejezet végi feladatok válaszaiból, 3C-29/33/37, és saját rövid levezetéssel):** vízszintes talajról, $y_0 = 0$ kezdőmagasságból:

| Mennyiség | Képlet |
|---|---|
| Pályagörbe | $y = (\operatorname{tg}\theta_0)\,x - \dfrac{g}{2\,(v_0\cos\theta_0)^2}\,x^2$ ← parabola |
| Hajítás távolsága (azonos szintre érkezésig) | $R = \dfrac{v_0^2\sin 2\theta_0}{g}$ |
| Legnagyobb magasság | $y_{\max} = \dfrac{v_0^2\sin^2\theta_0}{2g}$ |
| Repülési idő (azonos szintre) | $T = \dfrac{2v_0\sin\theta_0}{g}$ |

- A hajítás távolsága **$\theta_0 = 45^\circ$-nál a legnagyobb**. Két szög, amelyek összege $90^\circ$ (pl. $30^\circ$ és $60^\circ$), **ugyanakkora** távolságot ad.
- Levezetés röviden: $y = 0$ → $v_0\sin\theta_0 \cdot t - \tfrac12 g t^2 = 0 \Rightarrow t = 0$ vagy $t = \dfrac{2v_0\sin\theta_0}{g}$. Ezt $x$-be: $R = v_0\cos\theta_0\cdot\dfrac{2v_0\sin\theta_0}{g} = \dfrac{v_0^2\sin2\theta_0}{g}$ (mert $2\sin\theta\cos\theta = \sin2\theta$). A csúcson $v_y = 0$: $t = \dfrac{v_0\sin\theta_0}{g}$, ezt $y$-ba téve kapjuk $y_{\max}$-ot.
- A pályagörbét úgy kapod, hogy az $x = v_0\cos\theta_0\, t$-ből kifejezed $t$-t, és behelyettesíted $y$-ba.

#### Diákmankó (derékszögű háromszög és szögfüggvények)

```
            /|
           / |
        r /  |  y = r · sinθ      szemközti befogó
         /   |
        /θ   |
       /_____|
        x = r · cosθ              szög melletti befogó

   sinθ = y / r     cosθ = x / r     tgθ = y / x
```

- **Szinusz** = szemközti / átfogó; **koszinusz** = szög melletti / átfogó; **tangens** = szemközti / szög melletti.
- Takard le a keresettet (a háromszögnél: $x = r\cos\theta$, $y = r\sin\theta$, $r = x/\cos\theta$, $\operatorname{tg}\theta = y/x$).
- **Hasznos háromszög:** a **3-4-5** derékszögű háromszög hegyesszögei kb. **36,9°** és **53,1°**. Ezt érdemes fejben tartani.

**Vektorösszeadás-mankó:** *mindent bontsd komponensekre, add össze komponensenként, majd rakd vissza (Pitagorasz + arctg, negyed-szabály).*

#### Levezetések

**(a) Komponensek és polárkoordináták:** egy $(r,\theta)$ vektor végpontjából az $x$ tengelyre merőlegest bocsátunk. A kapott derékszögű háromszög átfogója $r$, a $\theta$ melletti befogó $x$, a szemközti befogó $y$. A szögfüggvények definíciójából: $\cos\theta = x/r$, $\sin\theta = y/r$, $\operatorname{tg}\theta = y/x$. Pitagorasz: $r^2 = x^2 + y^2$.

**(b) Elmozdulásvektor komponensei:** $\mathbf r_1 + \Delta\mathbf r = \mathbf r_2$, ezért $\Delta\mathbf r = \mathbf r_2 - \mathbf r_1$. Komponensenként: $\Delta x = x_2 - x_1$, $\Delta y = y_2 - y_1$.

**(c) A sebességvektor komponensei:** $\mathbf r = x\hat{\mathbf x} + y\hat{\mathbf y} + z\hat{\mathbf z}$-t idő szerint deriválva a szorzatszabály szerint adódik:
$$\mathbf v = \frac{dx}{dt}\hat{\mathbf x} + x\frac{d\hat{\mathbf x}}{dt} + \ldots$$
Az egységvektorok **állandók** (se nagyságuk, se irányuk nem változik az időben), ezért $\dfrac{d\hat{\mathbf x}}{dt} = \dfrac{d\hat{\mathbf y}}{dt} = \dfrac{d\hat{\mathbf z}}{dt} = 0$. Így $\mathbf v = v_x\hat{\mathbf x} + v_y\hat{\mathbf y} + v_z\hat{\mathbf z}$, ahol $v_x = dx/dt$ stb. Ugyanez a gyorsulásra: $a_x = dv_x/dt$ stb.

**(d) Miért érintő irányú a sebesség?** A $\Delta\mathbf r$ a két pontot összekötő húr iránya. Ha a második pontot egyre közelebb visszük az elsőhöz ($\Delta t\to0$), a húr iránya az első pontban húzott **érintő** irányához tart (3-20 ábra).

**(e) A hajítás levezetése:** az $\mathbf a = (0,\,-g)$ konstans gyorsulás komponenseit külön-külön az egyenesvonalú egyenletekbe írjuk:
- $x$ irányban $a_x = 0$ → egyenletes mozgás: $x = x_0 + v_0\cos\theta_0\,t$
- $y$ irányban $a_y = -g$ → állandó gyorsulású mozgás: $y = y_0 + v_0\sin\theta_0\,t - \tfrac12 gt^2$

---

### 2.3 Feladatok levezetése (a fejezet példái)

#### 3-1 példa: komponensek meghatározása
*Az $\mathbf r$ helyzetvektor nagysága 0,1 m, iránya 150°-os szöget zár be a pozitív $x$ tengellyel. Határozzuk meg a derékszögű komponenseit.*

- $x = r\cos150^\circ = (0{,}10\ \text{m})(-0{,}866) = \boxed{-0{,}0866\ \text{m}}$
- $y = r\sin150^\circ = (0{,}10\ \text{m})(0{,}5) = \boxed{0{,}0500\ \text{m}}$
- A vektor a **II. negyedben** van ($x<0,\ y>0$), ezért $x$ negatív. A szögfüggvények előjel-szabályai adják az előjeleket.
- **Tanulság:** a polárkoordinátáknál $\theta$-t a +x tengelytől, ellentétes óramutató irányban mérjük. Ha más tengelytől mért szöget is jelölsz az ábrán, az ábrából legyen világos, melyikről van szó.

#### 3-2 példa: elmozdulásvektor nagysága és iránya
*Egy részecske a $(2\ \text{m},\ 1\ \text{m})$ pontból az $(5\ \text{m},\ 5\ \text{m})$ pontba mozdul el.*

- $\Delta x = x_2 - x_1 = 5 - 2 = 3\ \text{m}$, $\Delta y = y_2 - y_1 = 5 - 1 = 4\ \text{m}$
- Nagyság (Pitagorasz): $|\Delta\mathbf r| = \sqrt{3^2 + 4^2} = \sqrt{25} = \boxed{5{,}00\ \text{m}}$ (3-4-5 háromszög)
- Irány: $\operatorname{tg}\theta = \dfrac{\Delta y}{\Delta x} = \dfrac{4}{3} = 1{,}33 \Rightarrow \theta = \operatorname{arc\,tg}1{,}33 = \boxed{53{,}1^\circ}$ az $x$ tengellyel

#### 3-3 példa: vektorösszeadás algebrailag
*$\mathbf A = (3\ \text{m})\hat{\mathbf x} + (3\ \text{m})\hat{\mathbf y}$, $\mathbf B = (1\ \text{m})\hat{\mathbf x} + (-4\ \text{m})\hat{\mathbf y}$, $\mathbf C = (-2\ \text{m})\hat{\mathbf x} + (3\ \text{m})\hat{\mathbf y}$. Határozzuk meg a) $\mathbf D = \mathbf A + \mathbf B + \mathbf C$, b) $\mathbf E = -\mathbf A - \mathbf B + \mathbf C$ vektort.*

**a)** Táblázat (komponensenként összeadunk):

| Vektor | $x$ komponens | $y$ komponens |
|---|---|---|
| $\mathbf A$ | 3 m | 3 m |
| $\mathbf B$ | 1 m | −4 m |
| $\mathbf C$ | −2 m | 5 m |
| $\mathbf D$ | **2 m** | **4 m** |

*(Figyelem: a feladatszövegben a $\mathbf C$ vektor $y$ komponense 3 m-nek látszik, a megoldás táblázata és az eredmények viszont 5 m-mel számolnak. Itt az 5 m-es értéket használom. Ellenőrizd a nyomtatott könyvben.)*

- $\mathbf D = (2\ \text{m})\hat{\mathbf x} + (4\ \text{m})\hat{\mathbf y}$
- $|\mathbf D| = \sqrt{2^2 + 4^2} = \sqrt{20} = \boxed{4{,}47\ \text{m}}$
- $\theta = \operatorname{arc\,tg}\dfrac{4}{2} = \operatorname{arc\,tg}2 = \boxed{63{,}4^\circ}$ (I. negyed)

**b)** $-\mathbf A$ és $-\mathbf B$ komponensei az $\mathbf A$ és $\mathbf B$ komponenseinek ellentettjei:

| Vektor | $x$ | $y$ |
|---|---|---|
| $-\mathbf A$ | −3 | −3 |
| $-\mathbf B$ | −1 | 4 |
| $\mathbf C$ | −2 | 5 |
| $\mathbf E$ | **−6** | **6** |

- $\mathbf E = (-6\ \text{m})\hat{\mathbf x} + (6\ \text{m})\hat{\mathbf y}$
- $|\mathbf E| = \sqrt{36 + 36} = \boxed{8{,}49\ \text{m}}$
- Hegyesszög a negatív $x$ tengellyel: $\varphi = \operatorname{arc\,tg}\left|\dfrac{6}{-6}\right| = 45^\circ$. A vektor a **II. negyedben** van, így $\theta = 180^\circ - 45^\circ = \boxed{135^\circ}$.

#### 3-4 példa: vektorok összeadása polárkoordinátákkal
*$\mathbf F = (4\ \text{m},\ 150^\circ)$ és $\mathbf G = (5\ \text{m},\ 270^\circ)$. Határozzuk meg $\mathbf H = \mathbf F + \mathbf G$ polárkoordinátáit.*

**Módszer:** először derékszögű komponensekre bontjuk, összeadjuk, majd vissza polárba.

| Vektor | $x$ komponens | $y$ komponens |
|---|---|---|
| $\mathbf F$ | $4\cos150^\circ = -3{,}464$ m | $4\sin150^\circ = 2{,}00$ m |
| $\mathbf G$ | $5\cos270^\circ = 0$ | $5\sin270^\circ = -5{,}00$ m |
| $\mathbf H$ | **−3,464 m** | **−3,00 m** |

> ⚠️ **Eltérés a PDF-ben:** a beolvasott táblázatban az $x$ komponens értéke (−3,142 és −3,646) elírásnak tűnik. $4\cos150^\circ$ valójában **−3,464**, és a későbbi számolás is ezzel dolgozik (a $\operatorname{tg}\varphi = 3{,}000/3{,}464 = 0{,}8661$ és $|\mathbf H| = 4{,}58$ m is ezt igazolja). Ellenőrizd a nyomtatott könyvben.

- $|\mathbf H| = \sqrt{3{,}464^2 + 3{,}00^2} = \sqrt{21} = \boxed{4{,}58\ \text{m}}$
- Hegyesszög az $x$ tengellyel: $\varphi = \operatorname{arc\,tg}\dfrac{3{,}000}{3{,}464} = \operatorname{arc\,tg}\,0{,}8661 = 40{,}9^\circ$
- A vektor a **III. negyedben** van ($x<0,\ y<0$) → $\theta = 180^\circ + 40{,}9^\circ = \boxed{221^\circ}$
- $\mathbf H = (4{,}58\ \text{m},\ 221^\circ)$
- **Tanulság:** a számológép $\operatorname{arc\,tg}$-je csak $-90^\circ\ldots90^\circ$-ot ad, ezért II. és III. negyedben **külön gonddal** kell eljárni. Mindig készíts ábrát!

#### 3-5 példa: térbeli elmozdulások (helikopter)
*A helikopter az állomásról $40^\circ$-os szögben **északkelet felé** (az északi iránytól keletre) indul, vízszintesen 2 km-t tesz meg, miközben a magassága 2500 m-re nő. Ezután **keletre** fordul, és 3 km-t megy vízszintesen, közben 1500 m magasságra süllyed. Milyen irányban és milyen távolságra jutott a reptértől?*

> A könyv megoldása és ábrája szerint a **végső magasság 1,5 km** (tehát a második szakaszon 1,0 km-t süllyed, $\Delta z = -1{,}0$ km). A feladat szövege a beolvasásban kicsit másként olvasható ("1500 m-t süllyedve"), ezért itt a megoldás szerinti értékekkel számolok.

**Koordinátarendszer:** $x$ = észak, $y$ = nyugat, $z$ = függőlegesen felfelé (km-ben).

| Vektor | $x$ (észak) | $y$ (nyugat) | $z$ (fel) |
|---|---|---|---|
| $\mathbf A$ (1. szakasz) | $2\cos40^\circ = 1{,}53$ | $-2\sin40^\circ = -1{,}29$ | $+2{,}5$ |
| $\mathbf B$ (2. szakasz, kelet) | 0 | $-3$ | $1{,}5 - 2{,}5 = -1{,}0$ |
| $\mathbf C = \mathbf A + \mathbf B$ | **1,53** | **−4,29** | **1,5** |

- $\mathbf C = 1{,}53\,\hat{\mathbf x} - 4{,}29\,\hat{\mathbf y} + 1{,}5\,\hat{\mathbf z}$ (km)
- **Távolság a reptértől:** $|\mathbf C| = \sqrt{1{,}53^2 + 4{,}29^2 + 1{,}50^2} = \boxed{4{,}79\ \text{km}}$
- **Vízszintes irány:** $\varphi = \operatorname{arc\,tg}\dfrac{4{,}29}{1{,}53} = \boxed{70{,}3^\circ}$ az északi iránytól keletre (a könyv „északkeletre" mondja, valójában inkább kelet-északkelet)
- **Vízszintes összetevő:** $C_{\text{vízsz}} = \sqrt{4{,}29^2 + 1{,}53^2} = 4{,}55$ km
- **Emelkedési szög:** $\psi = \operatorname{arc\,cos}\dfrac{4{,}55}{4{,}79} = \boxed{18{,}2^\circ}$ a **horizont felett**

#### 3-6 példa: sebességvektor komponensekből
*Egy részecske helyzetvektorának koordinátái $x = (2\ \text{m/s}^2)t^2$ és $y = (16\ \text{m·s}^2)/t^2$. Határozzuk meg a helyzetvektort és a sebességvektort $t = 2$ s-nál.*

- Helyzetvektor: $\mathbf r = 2t^2\,\hat{\mathbf x} + \dfrac{16}{t^2}\,\hat{\mathbf y}$ (SI-ben)
- Sebességvektor (deriválás komponensenként):
  $$\mathbf v = \frac{d\mathbf r}{dt} = 4t\,\hat{\mathbf x} - \frac{32}{t^3}\,\hat{\mathbf y}$$
  (Deriválás: $(2t^2)' = 4t$; $(16t^{-2})' = -32t^{-3}$.)
- $t = 2$ s-nál:
  - $\mathbf r = (8\,\hat{\mathbf x} + 4\,\hat{\mathbf y})\ \text{m}$
  - $\mathbf v = (8\,\hat{\mathbf x} - 4\,\hat{\mathbf y})\ \text{m/s}$

#### 3-7 példa: gyorsulásvektor
*Ugyanennek a testnek a gyorsulása $t = 2$ s-nál.*

- $\mathbf a = \dfrac{d\mathbf v}{dt} = \dfrac{d}{dt}\left(4t\,\hat{\mathbf x} - \dfrac{32}{t^3}\,\hat{\mathbf y}\right) = 4\,\hat{\mathbf x} + \dfrac{96}{t^4}\,\hat{\mathbf y}$
- $t = 2$ s: $\mathbf a = \boxed{(4\,\hat{\mathbf x} + 6\,\hat{\mathbf y})\ \text{m/s}^2}$
- Itt $\mathbf a$ iránya sem a $\mathbf v$, sem az $\mathbf r$ irányával nem egyezik meg.

#### 3-8 példa: lövedék dombra (ferde hajítás)
*Egy lövedéket a vízszinteshez képest $\theta_0 = 55^\circ$-os szögben, $v_0 = 50$ m/s sebességgel lőnek ki. A lövedék a kilövés helye fölött **60 m**-rel egy domboldalba csapódik. a) Mennyi ideig repül? b) A kilövés helyétől milyen vízszintes távolságban csapódik be? c) Mekkora sebességgel csapódik be?*

**Adatok** ($x_0 = y_0 = 0$, felfelé pozitív $y$):
- $(v_x)_0 = 50\cos55^\circ = 28{,}7$ m/s, $a_x = 0$
- $(v_y)_0 = 50\sin55^\circ = 41{,}0$ m/s, $a_y = -g = -9{,}81$ m/s², $y = 60$ m

**a) Idő** (az $y$ irányú egyenletből, mert ott minden ismert az időn kívül):
$$y = (v_y)_0\,t - \tfrac12 g t^2 \;\Rightarrow\; 60 = 41{,}0\,t - 4{,}905\,t^2$$
Rendezve: $4{,}905\,t^2 - 41{,}0\,t + 60 = 0$ → másodfokú megoldóképlet:
$$t = \frac{41{,}0 \pm \sqrt{41{,}0^2 - 4\cdot4{,}905\cdot60}}{2\cdot4{,}905} \;\Rightarrow\; t = 6{,}46\ \text{s}\ \ \text{vagy}\ \ t = 1{,}89\ \text{s}$$
- A $t = 1{,}89$ s a **felszálló ágban** jelenti a 60 m magasságot (a lövedék ekkor még emelkedik). A **becsapódás** a **leszálló ágban** van → $\boxed{t = 6{,}46\ \text{s}}$. (Itt mindkét gyök fizikailag létező időpont, de csak a második a becsapódás.)

**b) Távolság:** $x = (v_x)_0\,t = 28{,}7 \cdot 6{,}46 = \boxed{185\ \text{m}}$

**c) Becsapódási sebesség:**
- $v_x = 28{,}7$ m/s (állandó)
- $v_y = (v_y)_0 - g t = 41{,}0 - 9{,}81\cdot6{,}46 = -22{,}4$ m/s (negatív: lefelé mozog)
- $|\mathbf v| = \sqrt{28{,}7^2 + 22{,}4^2} = \boxed{36{,}4\ \text{m/s}}$
- Szög a vízszintessel: $\varphi = \operatorname{arc\,tg}\dfrac{22{,}4}{28{,}7} = \boxed{38{,}0^\circ}$ **lefelé**

**Tanulság:** nem kell a felfelé és lefelé repülést külön számolni. A kinematikai egyenlet a teljes mozgásra érvényes.

#### 3-9 példa: lefelé hajított labda ablakból
*Egy épület felső emeleti ablakából egy labdát $v_0 = 8$ m/s sebességgel, a vízszintessel $20^\circ$-os szöget bezáró irányban **lefelé** hajítunk el. A labda 3 s múlva csapódik a talajba. a) Az épület aljától milyen távolságra ér földet? b) Milyen magasról hajítottuk el? c) Mennyi idő telt el, míg a labda a kiindulási helyzeténél 10 m-rel lejjebb került?*

**Koordinátarendszer:** mivel minden mozgás lefelé irányul, a **lefelé** irányt választjuk pozitívnak → $a_y = +g$.
- $(v_x)_0 = 8\cos20^\circ = 7{,}52$ m/s, $a_x = 0$
- $(v_y)_0 = 8\sin20^\circ = 2{,}74$ m/s, $a_y = +9{,}8$ m/s²

**a)** $x = (v_x)_0\,t = 7{,}52\cdot3 = \boxed{22{,}6\ \text{m}}$

**b)** $y = (v_y)_0\,t + \tfrac12 a_y t^2 = 2{,}74\cdot3 + \tfrac12\cdot9{,}8\cdot3^2 = 8{,}2 + 44{,}1 \approx \boxed{52{,}3\ \text{m}}$ (g ≈ 9,8 m/s²-tel)

**c)** $y = 10$ m: $10 = 2{,}74\,t + 4{,}9\,t^2 \Rightarrow 4{,}90\,t^2 + 2{,}74\,t - 10 = 0$
$$t = \frac{-2{,}74 \pm \sqrt{2{,}74^2 + 4\cdot4{,}90\cdot10}}{2\cdot4{,}90} \;\Rightarrow\; t = +1{,}18\ \text{s}\ \text{vagy}\ t = -1{,}74\ \text{s}$$
- A negatív gyök a mozgás **kezdete előtti** időpont (a pálya elképzelt, korábbi szakasza) → **hamis gyök**, elvetjük.
- $\boxed{t = 1{,}18\ \text{s}}$

#### 3-10 példa: hajított test vektorfüggvényekkel
*Egy test helyvektora (SI-ben): $\mathbf r = (9{,}8\,t)\,\hat{\mathbf x} + (19{,}6\,t - 4{,}9\,t^2)\,\hat{\mathbf y}$. Határozzuk meg a helyzet-, sebesség- és gyorsulásvektort $t = 3$ s-nál.*

- **Helyzet:** $x = 9{,}8\cdot3 = 29{,}4$ m, $y = 19{,}6\cdot3 - 4{,}9\cdot9 = 58{,}8 - 44{,}1 = 14{,}7$ m
  - $\mathbf r(3) = (29{,}4\,\hat{\mathbf x} + 14{,}7\,\hat{\mathbf y})\ \text{m}$
  - $|\mathbf r| = \sqrt{29{,}4^2 + 14{,}7^2} = 32{,}9$ m. **Ez nem egyenlő a test által befutott pálya hosszával!**
  - Szög: $\operatorname{tg}\theta = 14{,}7/29{,}4 = 0{,}500 \Rightarrow \theta = 26{,}5^\circ$
- **Sebesség:** $\mathbf v = \dfrac{d\mathbf r}{dt} = 9{,}8\,\hat{\mathbf x} + (19{,}6 - 9{,}8\,t)\,\hat{\mathbf y}$
  - $t = 3$ s: $\mathbf v = (9{,}8\,\hat{\mathbf x} - 9{,}8\,\hat{\mathbf y})\ \text{m/s}$
  - $|\mathbf v| = \sqrt{9{,}8^2 + 9{,}8^2} \approx 13{,}9$ m/s, $\operatorname{tg}\varphi = 9{,}8/9{,}8 = 1 \Rightarrow \varphi = 45^\circ$ a horizont **alatt**
  - (Megjegyzés: $t = 2$ s-nál $v_y = 0$, de $v_x \ne 0$. A pálya csúcsán a test vízszintesen mozog.)
- **Gyorsulás:** $\mathbf a = \dfrac{d\mathbf v}{dt} = -9{,}8\,\hat{\mathbf y}\ \text{m/s}^2$, tehát az $y$ tengely **negatív** irányába mutat, és az időben **állandó**.

---

### 2.4 Egyszerű módja a téma megértésének

**A legfontosabb gondolat egy mondatban:**
*A kétdimenziós mozgás = két, egymástól független egydimenziós mozgás egyszerre.*

**Képzeld el így:**
- A **vektor egy nyíl**: a hossza a nagyság, a nyílhegy az irány. Két dimenzióban két számmal (komponens) adható meg: „mennyit megyek jobbra/balra, mennyit fel/le".
- **Összeadás = útvonalak egymás után:** először megyek az $\mathbf A$ nyíl mentén, aztán a $\mathbf B$ mentén. Az eredő útvonal a kezdőpontból a végpontba mutató nyíl.
- **Kivonás = az ellentett hozzáadása:** $\mathbf A - \mathbf B$ az $\mathbf A$-hoz hozzáadott „visszafelé $\mathbf B$".
- **Hajítás:** két mozgás fut egyszerre.
  - **Vízszintesen** nincs semmi, ami lassítaná vagy gyorsítaná (a légellenállást elhanyagoljuk) → **egyenletes sebesség**.
  - **Függőlegesen** a gravitáció húz lefelé → **állandó $g$ gyorsulás**, ugyanúgy, mintha csak felfelé dobtuk vagy leejtettük volna.
  - A kettő **nem zavarja egymást**: a vízszintesen elhajított golflabda ugyanolyan ütemben esik, mint az, amelyiket leejtjük (3-26 ábra).

**Hajítás megoldási recept:**
1. **Vázlat**, koordinátarendszer: válaszd meg az origót és a pozitív irányokat (általában $x$ vízszintesen, $y$ felfelé).
2. **Bontsd komponensekre** a kezdősebességet: $v_{0x} = v_0\cos\theta_0$, $v_{0y} = v_0\sin\theta_0$.
3. **Két külön „kis feladat":** $x$: $a=0$ (egyenletes mozgás). $y$: $a=-g$ (állandó gyorsulású mozgás).
4. **Az idő a közös ismeretlen.** Általában az $y$ irányú egyenletből számold ki (gyakran másodfokú, ellenőrizd a gyököket!), aztán helyettesítsd az $x$ irányúba.
5. A **végső sebességet** komponensenként számold, majd rakd össze: $|\mathbf v| = \sqrt{v_x^2 + v_y^2}$, szög: $\operatorname{arc\,tg}(|v_y|/|v_x|)$.
6. **Ellenőrizd:** értelmes az eredmény? Mindkét gyök fizikailag lehetséges? Egységek rendben?

**Gyakori hibák:**
- A gyorsulás iránya **nem** egyezik a mozgás irányával (hajításnál mindig lefelé mutat, bármerre is megy a test).
- A sebességvektor mindig a **pálya érintője**, nem a helyvektor irányába mutat.
- A pálya **csúcsán** ferde hajításnál a sebesség **nem nulla**, csak a függőleges összetevője az.
- $|\Delta\mathbf r|$ (elmozdulás nagysága) **nem** egyenlő a megtett úttal.
- Szög mérésénél tisztázd: melyik tengelytől mérjük? (Polárkoordinátáknál a +x tengelytől, ellentétes óramutató irányban.)
- II. és III. negyedben az $\operatorname{arc\,tg}$ eredményét **korrigálni kell** (negyed-szabály).
- Negatív előjelet vektorábrán csak ellentett vektor jelölésére használj.
- Ne keverd az irányokat: ha a lefelé irányt választod pozitívnak, akkor $a_y = +g$.

---

## 3. Téma lezárása

### Rövid emlékeztető: mit tanultunk?
- A **vektor** nagysággal és iránnyal rendelkező mennyiség. **Komponensekkel** egyértelműen megadható: $\mathbf C = C_x\hat{\mathbf x} + C_y\hat{\mathbf y} (+ C_z\hat{\mathbf z})$.
- **Koordinátarendszerek:** derékszögű $(x,y)$, polár $(r,\theta)$; $x = r\cos\theta$, $y = r\sin\theta$, $r = \sqrt{x^2+y^2}$. Térben jobbrendszert használunk, további rendszerek: henger- és gömbi koordináták.
- **Vektorok összeadása/kivonása:** geometriailag (nyilak egymás után), algebrailag **komponensenként**. Az összeadás kommutatív és asszociatív, a kivonás nem kommutatív.
- **Helyvektor** ($\mathbf r$) → **elmozdulás** ($\Delta\mathbf r = \mathbf r_2 - \mathbf r_1$) → **sebesség** ($\mathbf v = d\mathbf r/dt$, mindig a pálya érintője) → **gyorsulás** ($\mathbf a = d\mathbf v/dt$). Ezek iránya általában különbözik.
- Állandó gyorsulásnál az egyenesvonalú kinematikai egyenletek **komponensenként külön-külön** érvényesek.
- **Hajítás (Galilei):** a vízszintes és a függőleges mozgás független. Vízszintesen egyenletes, függőlegesen $a = -g$. A pálya parabola.

### Rövid befejezés
Az előző modulban megtanultuk leírni az egyenes vonalú mozgást, most pedig a vektorokkal már bármilyen síkbeli és térbeli mozgás leírható. A hajításnál láttuk, hogy a bonyolultnak tűnő pálya két egyszerű mozgásra bomlik. A vektoros gondolkodás minden további fejezetben vissza fog térni.

### Gyakorló feladatok a fejezet végén (a könyvből)
| Alfejezet | Feladatok |
|---|---|
| 3.4 Vektorok összeadása és kivonása | 3A-1 … 3B-6 |
| 3.5 Térbeli vektorok | 3A-7, 3A-8 |
| 3.6–3.7 Sebesség, gyorsulás, hajítások | 3B-9 … 3B-24 (köztük 3A-14, 3A-15) |
| További feladatok | 3C-25 … 3C-40 |

- A **3C-29, 3C-31, 3C-33, 3C-35, 3C-37, 3C-39** feladatok a hajítás általános összefüggéseit vezetik le (távolság, legnagyobb magasság, pályagörbe). Az összefoglalóban a fontosabb eredményeket a kiegészítésnél leírtam.
- A **kérdések (1–9)** fogalmi gyakorlásra valók (pl. az idő vektormennyiség-e, mikor lehet három vektor eredője nulla, hajó árbocáról leejtett kő, a mozgás mennyiségeinek irányai).
- A **páratlan sorszámú feladatok** megoldása a könyv végén található (III. fejezet).

### ➡️ Következő modul
**Körmozgás:** [[kormozgas]]
