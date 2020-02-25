# FlexBox

1. preferable image should be block or inline block element, otherwise there will be space between images.
2. When we say magin auto it occupy the place which needs itself but look like occupy more than it looks. Basically all the space untill next element.
3. We can use currentColor value to use the same color in the element. Advantage of it is that when we change color for example on hover, we can change only color, then where we used currentColor will be changed.

```
.btn-inline {
  border: none;
  color: var(--color-primary);
  font-size: inherit;
  border-bottom: 1px solid currentColor;
}
.btn-inline:hover {
  color: var(--color-grey-dark-1);
}

```
