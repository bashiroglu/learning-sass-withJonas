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

adding support for older browsers

```
    // Older browsers 
    background-image: url(../img/chevron-thin-right.svg);
    background-size: cover;

    //Newer browsers - masks
    @supports (-webkit-mask-image: url()) or (mask-image: url()) {
      background-color: var(--color-primary);
      -webkit-mask-image: url(../img/chevron-thin-right.svg);
      -webkit-mask-size: cover;
      mask-image: url(../img/chevron-thin-right.svg);
      mask-size: cover;
      background-image: none; // we say bg-img none because otherwise it will be the same code
      // and the mask wouldn't be implemented.
    }
```
