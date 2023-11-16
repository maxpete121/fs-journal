# Bootstrap

Bootstrap can be called a library or framework

Classes

container is a class you can set on elements
fluid container spreads the whole page
container does not

Row Border - Will align any item inside of it and make its width 100
row is not generally used to hold elements
 class column can be added to elements inside of row to make them take a column format

LIGHT or DARK will change color to white or black
 EXAMPLES
Change color
<section class="col-6 border-bottom border-light">

change position of text
<section class="text-end">

Change font size or width
<section class="fs-4 fw bold">

Button or change button
<section class="btn btn-dark">

Title Tag will display title when mouse hovers over element
<section title="keep it simple stupid">

hide elements
d-md-none = hidden
d-lg-block = visible

change a card w

BREAKING DOWN COLUMNS
nest a row inside of a column to break the original row into multiple sections
 
Price slider
<input name="price" type="range" class="form-range">

Hold an element in place on the page
will stop the element at the top of the page
<form class="sticky-top">
In style css use top, 100px; ect. to hold the element below the top of the page

form control
<select name="size" class="form-control">
 <option value="">small</option>
</select>

check box
<div class="form-check-label"><input type="checkbox" class="form-checkbox">checkbox title</div>

Offset column from side of the screen
<section class="column offset-1">

SET an image to size to its container
class="image-fluid"

size an image manually
class="w-50"

Set background to transparent
class="bs-bg-opacity: 5"



Display flex for boot
class="d-flex flex-column align items center"

Center image and tex
text-center

 DEBUG SCRIPT
 type script
 put class debug on element that needs it

 Size an image to its original
 class="object-fit-contain"

dissaper on screen resize
example
d-md-block
d-lg-none

class="row d-none d-md-flex"

REsize elements on page resize
class="col-12 col-md-7"

ORDER THINGS ON A PAGE
Parent class: class="order 1 order-md-0"
 
class="col-12 order 0"
class="col-6 order 1"

Round an image
<section class="round">
Basic Setup
 <section class="container">
   container
   <section class="container-fluid bg-white">
<div class="Row">
   <section class="column"><section>
   <div>
adding a number will space the columns
 <section class="col-6 bg primary">
 bg -- primary
       secondary
       warning
       danger

M-1/9 will space rows or columns out
<section>

set sizes on different screens
We will most comonly use medium or md, and large or lg
                    size                   
<section class="col-sm-4                col-md-2">


    PADDING
p- any
p-1
p-2
ect.

  