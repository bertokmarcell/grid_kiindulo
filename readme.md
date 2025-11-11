# CSS Grid rövid magyarázat

### `display: grid`
- Ezzel az elemet **grid konténerré** tesszük.
- A benne lévő gyerek elemek **rács cellákba** kerülnek.

### `justify content`
- középre teszi az elemeket

### `alight content`
- Ezzel az elemet **grid konténerré** tesszük.
- A benne lévő gyerek elemek **rács cellákba** kerülnek.

### `grid-template-columns` / `grid-template-rows`
- Meghatározza a **grid oszlopait és sorait**.
- Például: `grid-template-columns: 1fr 2fr;`  
  → az első oszlop 1 rész, a második 2 rész széles.

### `grid-auto-flow: column`
- Meghatározza, hogy a gyerek elemek **horizontálisan vagy vertikálisan** helyezkedjenek el.
- `column` → egymás mellé, sorba.

### `grid-template-areas`
- rács cellákhoz **neveket adhatunk**, és később könnyen elhelyezhetjük az elemeket.
- Például:
  ```css
### `align-items`
- Meghatározza, hogy a **grid vagy flex gyerek elemek** hogyan helyezkedjenek el **vertikálisan** a cellákon belül.  
- Példák:
  - `align-items: start;` → tetejére igazítva
  - `align-items: center;` → középre
  - `align-items: end;` → aljára

### `grid-template-columns: repeat(auto-fill, minmax(200px, 1fr))`
- Automatikusan létrehoz **oszlopokat**, amelyek **legalább 200px szélesek**, de ha van hely, **növekedhetnek** (max 1fr).  
- `repeat(auto-fill, ...)` → annyi oszlop jön létre, amennyi elfér a konténer szélességében.  
- Ez **rugalmas, reszponzív grid-et** hoz létre: az oszlopok száma automatikusan változik az elérhető helytől függően.

  grid-template-areas: 
    "header header"
    "nav article"
    "footer footer";