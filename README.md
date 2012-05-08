# Choreographic Grid
### A CSS grid for content interdigitation
After having read Trent Walton's article on [Content Choreography](http://trentwalton.com/2011/07/14/content-choreography/) & working on a number of responsive sites, I felt that the current group of CSS grids was lacking in this department - so I [created my own](https://github.com/mrmartineau/Choreographic-Grid).

It is definitely a work in progress & there are still features I would like to add but I thought I should get a sense check from you guys to see if its worth pursuing.

As well as the [usual grid](http://mrmartineau.github.com/Choreographic-Grid/test.html#standard), [centred columns](http://mrmartineau.github.com/Choreographic-Grid/test.html#centred), [source ordering](http://mrmartineau.github.com/Choreographic-Grid/test.html#source-ordering) & [offsetting](http://mrmartineau.github.com/Choreographic-Grid/test.html#offset), I have added two features: **Shunting** & **Splitting**.

## Shunts ([demo link](http://mrmartineau.github.com/Choreographic-Grid/test.html#shunt))
**Shunts** are, typically, small columns on the end of a row that 'shunt' down to their own row when the viewport dimensions are reduced. The other columns in that row can then be resized to fill the leftover space from the shunted column.

## Splits ([demo link](http://mrmartineau.github.com/Choreographic-Grid/test.html#split))
**Splits**  are columns that sit beside each other on wider viewports but when the viewport dimensions are reduced, they stack on top of each other. This might seem like 'normal' responsive grid behaviour but the rest of the grid is still enforced (for want of a better word).

Both these things allow the layout to adapt in a more natural way, that traditionally has not been available to us.

By the way, **Splits** can be shunted too.

I should caveat this by saying that there is lots more work to be done, I have repeated some code in different media-queries which I don't want to do - I have big plans for this grid. I'm also not using CSS that only works in Chrome Canary, you can use this today if you wanted to.

One feature that I would like to implement is to automatically name each media-query. I want to use javascript to find all the breakpoints & then store them in an array, then add a class to the body tag so I can change layout depending on how wide the viewport is. I like the idea of naming media-queries so I will explore the possibilities in the coming weeks.

**If anyone has any thoughts, ideas or suggestions I would really appreciate it.  Please [fork it](https://github.com/mrmartineau/Choreographic-Grid) too**

[Demo site](http://mrmartineau.github.com/Choreographic-Grid/test.html) - [http://mrmartineau.github.com/Choreographic-Grid/test.html](http://mrmartineau.github.com/Choreographic-Grid/test.html)

[All features on one page](http://mrmartineau.github.com/Choreographic-Grid/index.html) - [http://mrmartineau.github.com/Choreographic-Grid/index.html](http://mrmartineau.github.com/Choreographic-Grid/index.html)