## Grid intro

Grid allows use to create two-dimensional layout

```
.container {
  background: rgb(159, 160, 81);
  display: grid;
  margin: 35px auto;
  gap: 25px;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 200px);
}
.item {
  background: rgb(201, 79, 79);
}
/* .item-2 {
  grid-row: 1/2;
  grid-column: 1/3;
} */
.item-1 {
  grid-row: 1 / 2;
  grid-column: 1 / span 4;
}
```

- We start our grid layout by defining rows
- Then we continue with columns
- When we define column we can use minmax which means max second argument but never small than first argument
  for example:

```
minmax(min-content, 10rem)
```

- When we want to give height to row that will adjust content we ca give it to min-content or auto
- When we use -1, it works only with explict grid not with implicit grid.
- Auto-fit value means, you can wrap as much as your parent width or height.
- Imgs are like exceptional for grid they preserve their dimensions, that is why they don't fill all the grid area.
- When we want our image overlap grid, we can use scale or bigger percentage.
- If we want to grid item, over of each other, we can give the same place to both.
- in grid objectfit cover is like bg-size cover.
