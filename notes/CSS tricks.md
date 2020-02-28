## CSS tricks

If we want to have different styled and stunning text with the gradient background we can use the rtick below:

```
.text{
    display: inline-block;
    background-image: linear-gradient(to right, $color-primary-light, $color-primary-dark);
    -webkit-background-clip: text;
    color: transparent;
}
```
