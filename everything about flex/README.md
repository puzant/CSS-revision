### Flex display property

#### Properties for the Parent(Flex container)

- `Display: flex`, defined a flex container, enabling flex context for all the children
```
.container {
  display: flex;
}
```

- `flex-direction: row | row-reverse | column | column-reverse`, specify the main axis, flex items can be

aligned either in horizontal rows or vertical columns 
``` 
.container {
  flex-direction: row;  //  align items in horzontal row
}
```
- `flex-wrap: wrap | nowrap | wrap-reverse`, flex items will try to fit in one line, `flex-wrap` makes
the element wrap to a new line

- `nowrap`: elements will be on the same line
- `wrap`: elements will be wrap into multiple lines
- `wrap-reverse`: similiar to `wrap` but from bottom to top

```
.container {
  flex-wrap: wrap
}
```

- `flex-flow`: this is a shorthand for `flex-direction` & `flex-wrap`, the default value is: `row nowrap`
```
.container {
  flex-flow: column wrap
}
```

- `justify-content`: defines the alignment along the main axis
> there are 5 values for this property:
1. `flex-strat`: itemes are aligned to the start line 
2. `flex-end`: itemes are aligned towards the end line 
3. `center`: itemes are aligned to the center 
4. `space-between`: items are evenly distributed in the line
5. `space-around`: items are evenly distributed in the line with equal spaces around them
6. `space-evenly`: items are distributed so that spacing between any two items is equal


- `align-items`: define the default behavior for how flex items are laid along the cross axis on the current line
> there are 6 values for the property
1. `stretch`: stretch to fill the container
2. `flex-start`: cross-start margin edge of the item is placed on the cross start line
3. `flex-end`: cross-end margin edge of the itme is placed on the cross-end line 
4. `center`: items are centered in the cross-axis
5. `baseline`: items are aligned such as thier baselines align 

- `align-content`: align's flex container's lines within when there an extra space in the cross axis
> there are 5 values for the property
1. `flex-start`: lines are packed to the start of the container 
2. `flex-end`: lines are packed to the end of the container 
3. `center`: lines are packed to the center
4. `space-between`: lines are evenly distributed, the first line is in start of the container, last line is at the end
5. `space-around`: lines evenly distributed with equal space around each line
6. `stretch`: lines stretch to take up the remaning space 


#### Properties for the Children(Flex items)
- `order`: by default flex items are laid out in source order

```
.flex-item {
  order: <integer> // default is 0
}
```

- `flex-grow`: defined the ability for a flex item to grow if necessary

> if all items have `flex-grow` set to 1, the remaning space in the container will be distributed equally
```
.flex-item {
  flex-grow: <number> //  default is 0
}
```

- `flex-shrink`: defines the ability for a flex item tow shrink if necessary

> negative numbers are invalid

```
.flex-item {
  flex-shrink: <number> //  default is 1
}
```

- `flex-basis`: defines the default size of an element before the remaning space is distributed

```
.flex-item {
  flex-basis: <length> | auto
}
```

- `flex`: this is a shorthand for `flex-grow` & `flex-shrink` & `flex-basis` combined, the second & third parameters are optional, default is 0

```
.flex-item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```

- `align-self`: this allows the default alignment to be overriden for individual flex-items

```
.flex-item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch
}
```