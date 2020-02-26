# CSS theory

#### Six stages of value

In css values are processed in six stages.

1. Declared value: the value which is declared by author
2. Cascaded value: the value which is chosen after conflicts
3. Specified value: in font size if there is not, it will be inherited ,if there is not (in padding or other not inherited values) any value from this stage value will be equal to 0.
4. Computed value: Relative values converted to pxs
5. Used value: final calculation
6. Actual value: happens in rendering stage and rounded somehow.

#### em and rem, other relative values

- In fonts sizes, percentage values will be relative to parent's computed font-size.
- In length sizes, percentage values will be relative to parent's computed width sizes.

- In fonts sizes, em values will be relative to parent's computed font-size.
- In length sizes, em values will be relative to its own computed font-size.
- In length sizes and fonts sizes, rem values will be relative to its root font-size.

  - Rem is always relative to root font size.

- vh and vw is easy,

#### inheritance

- font sizes and font related codes will be inherited from their parents, but not lengths like padding margin etc.

- computed value inrehits not declared value.

#### Box types 

block: line-break, 100% of parent with, normal box-model
inline: no height or width, occupy content's place, normal box-model
inline-block: , inline(left and right) box-model