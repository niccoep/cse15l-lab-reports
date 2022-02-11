# Lab report 2
***
We first checked if the md file has a 
The link to the commits is [here](https://github.com/niccoep/markdown-parse/commit/470feae778dfea41cb372677b6e3e39416a4fefa).
***
[Image](md_images/commits.png)
I rewrote some of the logic to make it more concise.

The first code change was checking for a ! at the index before the nextOpenBracket. This would make sure to not print images as images have a ```!``` before the first bracket.
***
A new bug arose when cheking the ```charAt(nextOpenBracket - 1)``` which would throw IndexOutOfBounds if the first bracket was the first char of the file.
***
A third bug was when the syntax for a link was not complet or broken e.g:
```[)``` or ```]]]```etc...

To fix this we check that each ```int``` storing a bracket index had been assigned. if not then ```break```