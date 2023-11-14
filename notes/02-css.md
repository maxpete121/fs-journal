# CSS
How to call to an element:
body {
background
}

link CSS
 <link rel="stylesheet" href="style.css">

 
Header Setup 
 
Each button in a header is its own element
- - can group navigation bar elements together


Margin and Padding are hard set
Flex allows the page to move with the viewport and is not hard set
padding X px Y px
padding 0 40px,

DISPLAY FLEX or FLEX CONTAINER
Loads elements side to side instead of top to bottom
EXAMPLE
.class {
    display: flex
    flex-direction: row/ row reverse
    justify-content: space evenly
}
NEED FLEX ELEMENTS TOP TO BOTTOM
use flex direction if elements are not block and need to be in column
column

All JC options x axis
space evenly
flex start- puts tags at begining of element
flex end - does the oposite of start
space evenly - moves all effected elements into the free space around the main element evenly

Align items y axis



CALL TO CLASS .example
CALL TO AN ID #example
CALL TO AN ELEMENT example
Target element inside of element
example
Div>span {
    background
}
Target class inside element
.class>div {
    color: orange
}
targets an element that has multiple twins in a larger element

header>div:nth-of-type(number of element)

When setting border
Use <hr/> to indicate content breaks
border-bottom solid 2px;


IMAGE ADJUSTING
set image class or just style img
object position (center)
object-fit: (cover)
width to 100% will make image fit to the page
height will do the same as width but horizontaly

 GENERAL NOTES

 Use icon library Class="mdi mdi-example"

 split lots of content into muliple boxes if possible
 if 2 sections set both width to 50%

 To span full page with a div set width to 100%

 min-height will allow elements to grow around inner tags

 Background will not show up unless tags have elements inside them

 set utility classes
 ex.
 .w-50 {
    width: 50%
 }
 .c-blue {
    color: blue;
 }

 Specificity is the order in which styles are specified
 
 Always link stylesheet last so it has a higher specificity then other links
 
 Can use
 margin-top or bottom
 padding-top or bottom


