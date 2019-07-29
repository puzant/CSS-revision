# Everything about CSS

## Selectors

1. `*`.................selects all the elements
2. `div`...............selects all the div tags
3. `div,p`.............selects all the div's & paragraphs
4. `div p`.............selects paragraphs inside divs
5. `div > p`...........selects all paragraphs, one level deep in div
6. `div + p`...........selects p tags immediately after div's
7. `div ~ p`...........selects p tags preceded by div 
8. `.classname`........select element with Class name
9. `#idname`...........select element with Id
10. `div.classname`....select divs with certain Class name
11. `div#idname`.......select div with certain Id name
12. `#idname*`.........select all the elements inside `#idname`

### Pseudo classes selectors

1. `a:link`....................link in normal state
2. `a:active`..................link in clicke state
3. `a:hover`...................link in hover state
4. `a:visited`.................already clicked link (visited)
5. `p::after{content:"foo"}`...add content after `p` element
6. `p::before`.................add content before `p` element
7. `input:checked`.............select checked input
8. `input:disabled`............select disabled input
9. `input:enabled`.............select enabled input(s)
10. `input:focus`..............input is in focus state
11. `input:in-range`...........input is in range
12. `input:out-of-range`.......input is out of range
13. `input:valid`..............input with valid values
14. `input:invalid`............input with invalid values
15. `input:optional`...........input with no required attributes
16. `input:read-only`..........input with readonly attribute
17. `input:read-only`..........input with no readonly attribute
18. `div:empty`................elements with no children
19. `p::first-letter`..........first letter in p
20. `p::first-line`............first line in p
21. `p:first-of-type`..........first of some type
22. `p:last-of-type`...........last of some type
23. `p:lang(en)`...............p with en language attribute
24. `:not(span)`...............element that's not a span
25. `p:first-child`............first child of its parent
26. `p:last-child`.............last child of its parent
27. `p:nth-child(2)`...........second child of its parent
28. `p:nth-child(3n+1)`........nth-child (an + b) formula
29. `p:nth-last-child(2)`......second child from behind
30. `p:nth-of-type(2)`.........second p of its parent
31. `p:nth-last-of-type(2)`....scond childfrom behind
32. `p:only-of-type`...........unique of its parent
33. `p:only-child`.............only child of its parent
34. `:root documents`..........root element
35. `::selection`..............portion selected by user
36. `:target`..................highlight active anchor

### Attribute selectors
1. `a[target]`...............link with a target attribute
2. `a[target="_blank"`.......link which opens in new tab
3. `[title="chair]`..........title elements with a word
4. `[class^="chair]`.........class name that starts with chair
5. `[class|="chair"]`........class start the chair word
6. `[class*="chair"]`........class contains chair
7. `[class$="chair"]`........class ends with chair
8. `input[type="button"]`....select an input with type button
