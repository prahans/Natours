Natours
lean about atomic design from this youtube video -> https://youtu.be/Yi-A20x2dcA?si=FQaVaMYF7OT_T4kq

BEM -> Block Element Modifier 
BLOCK : standalone component that is meaningful on its own.
ELEMENT : part of a block that has no standalone meaning.
MODIFIER : a different version of a block or element.

.block {}
.block__element {}
.block__element--modifier {}

* ARCHITECT
THE 7-1 PATTERN
7 different folders for partial Sass files, and
1 main Sass file to import all others files into a compiled CSS stylesheet.

THE 7 FOLDERS
.base/
.components/
.layout/
.pages/
.themes/
.abstracts/
.vendors/