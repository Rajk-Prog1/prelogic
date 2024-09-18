---
title: Prelogika
marp: true
math: mathjax
class: lead
paginate: false
footer: Prog1 - Prelogika
size: 16:9
theme: uncover
---

# Prelogika

---

## Mi a formális logika?

---

## Mi a formális logika?

Szimbólumok szabályos összefűzésével formált, jelentéssel bíró kifejezések rendszere. $\implies$ **NYELV**

A szimbólumok sorrendjét egyfajta nyelvtan, míg a keletkező kifejezések igazságtartalmát a logikai következtetés szabályai rögzítik.

---

## Ítéletlogika

- logikai változókkal és a velük elvégezhető műveletekkel foglalkozik
- logikai változó: csak az **IGAZ** és **HAMIS** értékeket veheti fel
- ilyen pl. egy állítás vagy egy matematikai kifejezés igazságértéke
- a logikai változók között - más típusú változókhoz hasonlóan - létezhetnek logikai műveletek

---

## Milyen értéke nem lehet logikai változónak?

---

## Milyen értéke nem lehet logikai változónak?

- 3
- "malac"
- "nem tudom"
- "attól függ"

---

## A formális logika két részre osztja a világot

---

## Alakítsd át logikai változóvá!

Nem logikai változó: Az eső valószínűsége (0%-tól 100%-ig bármi lehet az értéke)

A fentiből képzett logikai változó, amely igaz, ha...

1. Az eső valószínűsége nagyobb, mint 50%:

---

## Alakítsd át logikai változóvá!

1. Az eső valószínűsége nagyobb, mint 50%:
   Valószínűbb, hogy esni fog, mint hogy nem fog esni?

2. Az eső valószínűsége 100%, különben hamis:

---

## Alakítsd át logikai változóvá!

1. Az eső valószínűsége nagyobb, mint 50%:
   Valószínűbb, hogy esni fog, mint hogy nem fog esni?

2. Az eső valószínűsége 100%, különben hamis:
   Biztosan esni fog?

---

## Műveletek

¬: tagadás
∧: és (konjukció)
∨: vagy (diszjunkció)
⊕: kizáró vagy
⇒: implikáció
⇔: ekvivalencia

---

## Példák

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

1. Misi szereti a kevertet és részt vesz az Ábel kupán

---

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

1. Misi szereti a kevertet és részt vesz az Ábel kupán
   A ∧ B
2. Misi nem szereti a kevertet, de részt vesz az Ábel kupán

---

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

2. Misi nem szereti a kevertet, de részt vesz az Ábel kupán
   ¬ A ∧ B
3. Ha kevesen szeretik a kevertet és Misi szereti, akkor Misi rajkos

---

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

3. Ha kevesen szeretik a kevertet és Misi szereti, akkor Misi rajkos
   (D ∧ A) ⇒ C
4. Misi vagy nem rajkos, vagy szereti a kevertet és részt vesz az Ábel kupán

---

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

4. Misi vagy nem rajkos, vagy szereti a kevertet és részt vesz az Ábel kupán
   ¬ C ⊕ (A ∧ B) VAGY ¬ C ∨ (A ∧ B)
5. Misi akkor és csak akkor vesz részt az Ábel kupán, ha vagy szereti a kevertet, vagy rajkos

---

A: Misi szereti a kevertet, B: Misi részt vesz az Ábel kupán, C: Misi rajkos, D: kevesen szeretik a kevertet

5. Misi akkor és csak akkor vesz részt az Ábel kupán, ha vagy szereti a kevertet, vagy rajkos
   B ⇔ (A ∨ C)

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   |     |       |       |       |       |       |
| 1   | 0   |     |       |       |       |       |       |
| 0   | 1   |     |       |       |       |       |       |
| 0   | 0   |     |       |       |       |       |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   |       |       |       |       |       |
| 1   | 0   | 0   |       |       |       |       |       |
| 0   | 1   | 1   |       |       |       |       |       |
| 0   | 0   | 1   |       |       |       |       |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   | 1     |       |       |       |       |
| 1   | 0   | 0   | 0     |       |       |       |       |
| 0   | 1   | 1   | 0     |       |       |       |       |
| 0   | 0   | 1   | 0     |       |       |       |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   | 1     | 1     |       |       |       |
| 1   | 0   | 0   | 0     | 1     |       |       |       |
| 0   | 1   | 1   | 0     | 1     |       |       |       |
| 0   | 0   | 1   | 0     | 0     |       |       |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   | 1     | 1     | 0     |       |       |
| 1   | 0   | 0   | 0     | 1     | 1     |       |       |
| 0   | 1   | 1   | 0     | 1     | 1     |       |       |
| 0   | 0   | 1   | 0     | 0     | 0     |       |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   | 1     | 1     | 0     | 1     |       |
| 1   | 0   | 0   | 0     | 1     | 1     | 0     |       |
| 0   | 1   | 1   | 0     | 1     | 1     | 1     |       |
| 0   | 0   | 1   | 0     | 0     | 0     | 1     |       |

---

### Igazságtábla

| A   | B   | ¬A  | A ∧ B | A ∨ B | A ⊕ B | A ⇒ B | A ⇔ B |
| --- | --- | --- | ----- | ----- | ----- | ----- | ----- |
| 1   | 1   | 0   | 1     | 1     | 0     | 1     | 1     |
| 1   | 0   | 0   | 0     | 1     | 1     | 0     | 0     |
| 0   | 1   | 1   | 0     | 1     | 1     | 1     | 0     |
| 0   | 0   | 1   | 0     | 0     | 0     | 1     | 1     |

---

## Félösszeadó

Az ALU (arithmetic processing unit) egyszerű számításokat végző áramkör, a számítógépek processzorának alapköve. Ennek egyik komponense a félösszeadó, ami bináris számokat ad össze.

---

## ![half adder](./img/half_adder.png)

---

## Mire hasonlít mindez?

- változók
- meghatározott lehetséges értékek amiket változó felvehet
- változók közötti műveletek

---

## Mire hasonlít mindez?

- változók
- meghatározott lehetséges értékek amiket változó felvehet
- változók közötti műveletek

## Algebra

---

## Mik ezek?

- $x×0=0$
- $y^0=1$
- $(a+b)2=a2+2ab+b2$

---

## Mik ezek?

- $x×0=0$
- $y^0=1$
- $(a+b)2=a2+2ab+b2$

## Tételek

---

## Tételek

Olyan formulák, melyek a bennük szereplő változók értékétől függetlenül igazak

asszociativitás:

A∨(B∨C)⇔(A∨B)∨C

disztributivitás:

A∧(B∨C)⇔(A∧B)∨(A∧C)

---

## Tételek

Olyan formulák, melyek a bennük szereplő változók értékétől függetlenül igazak

De Morgan szabály:

¬(A∨B)⇔¬A∧¬B

szillogizmus:

(A⇒B)∧(B⇒C)⇒(A⇒C)

---

## Tétel-e?

1. A⇒B⇔¬A∨B

2. (A⇒B)∨(B⇒A)

---

## Szünet előtti játék

Annyit tudtok rólam, hogy vagy mindig az igazat mondom, vagy hazudok. _Feldobok egy érmét, amit csak én látok._

**Az eredmény akkor és csak akkor fej (vagy írás, a dobástól függ), ha igazmondó vagyok. Mi az érmefeldobás eredménye?**

---

## Megoldás igazságtáblával

A: Az eredmény fej (vagy írás).

B: Igazmondó vagyok.

Az állítás: $A \iff B$

| A   | B   | $A \iff B$ |
| --- | --- | ---------- |
| I   | I   | I          |
| I   | H   | H          |
| H   | I   | H          |
| H   | H   | I          |

---

Amit még tudunk, hogy: $B \iff (A \iff B)$. Ez mely esetekben igaz?

| A   | B   | $A\iff B$ | $B \iff (A \iff B)$ |
| --- | --- | --------- | ------------------- |
| I   | I   | I         | I                   |
| I   | H   | H         | I                   |
| H   | I   | H         | H                   |
| H   | H   | I         | H                   |

**Tehát csak az első két sor lehetséges, és mindkettőben A igaz, tehát biztosan fejet (vagy írást) dobtam. Hogy hazug, vagy igazmondó vagyok-e, irreleváns.**

---

## Elsőrendű logika

1. Predikátumok

- paraméter(eke)t tartalmazó kifejezés
- a benne szereplő paraméter(ek)től függ az igazságértéke

2. Kvantorok

- ∀ "mindegyik"
- ∃ "létezik"

---

##

## Predikátumok

1. egyváltozós

   - P: "páros szám"
   - P(x) akkor igaz ha x páros

2. többváltozós
   - NE: "nagyobb egyenlő"

- NE(x,y) akkor igaz ha x≥y, különben hamis

---

## Predikátumok

3. formulában
   - NE(x,y)∧P(y)
   - NE(x,y)⇒NE(y,x)

---

## Kvantorok

1. ∀
2. ∃

---

## Kvantorok formulában:

1. ∀x(P(2x))
2. ∀x(∃y(NE(x,y)))
3. ∄x(¬NE(x,x))

---

## Nyitott és zárt formulák

Ha egy kijelentésben egy paraméter minden előfordulása valamilyen kvantor hatáskörében van, akkor azt mondjuk, hogy a paraméter kötött, különben szabad.

Az a formula, aminek nincs szabad paramétere, zárt formula. Máskülönben nyitott formula.

---

## Példák

F(x): x férfi, N(x): x nő, V(x,y): x vonzónak tartja y-t

1. d-nek minden nő tetszik
2. k egy biszexuális nő
3. léteznek aszexuális emberek
4. mindenki biszexuális
5. csak a férfiak között vannak melegek

---
