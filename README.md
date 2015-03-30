# css-ratio [(demo)](http://codepen.io/entozoon/pen/yywxRz?editors=110 )

A simple CSS trick to let you give any block element a height that will keep it's given ratio responsively.

For example, it means you can use a background-image instead of an <img> element, or even an absolute positioned element and it will hold it's shape.


### Support
Any modern browser
IE8 - if you use the provided filter

### Usage
Have a look at the examples in this repository or see this [demo on codepen](http://codepen.io/entozoon/pen/yywxRz?editors=110 ).

### Changing Ratio
In the example it has a 16:9 ratio - which works by padding the bottom of the element by 56.25% of it's own width.

I.E. for 16:9, if you calculate 9/16 you get 0.5625 (which is 56.25%)

If you wanted 4:3, you would use padding-bottom: 75%;


Here are some common examples:
1:1  - padding-bottom: 100%;
4:3  - padding-bottom: 75%;
16:9 - padding-bottom: 56.25%;
3:2  - padding-bottom: 66.667%;
21:9 - padding-bottom: 42.857%;
3:1  - padding-bottom: 33.333%;

### Sass Mixin
This could be easily made into a sass mixin, wherein you'd provide the image url and a ratio.. the rest would be generated for you. Let me know if that's something you'd like to see.