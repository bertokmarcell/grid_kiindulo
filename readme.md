# CSS Grid rövid magyarázat

### `display: grid`
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
  grid-template-areas: 
    "header header"
    "nav article"
    "footer footer";