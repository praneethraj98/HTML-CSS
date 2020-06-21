The FlexBox container can be anything (div,ul,section)

Each direct child (div,img,li,h123) will be flex items
As long as anything is a direct child of the flex container, its going to be put into FlexBox

display: flex; automatically aligns the items
flex-direction: row/column/row-reverse/column-reverse are used to align items differently
flex: wrap; is used so that after the screen reaches a minimum size, the items are shifted onto the next row


.....................Flex Properties................

1. flex-shrink

.item-1 {
      flex-shrink: 0;
    }

item 1 doen not shrink even when the screen size is reduced

2. flex-grow and flex-basis

.item-2 {
      flex-grow: 1; 
      flex-basis: 0;          
    }
     -> fills up the remaining space of the container with item 2
.item-3 {
      flex-grow: 2;
      flex-basis: 0;           
    }
    -> fills up remaining space of the container with item 2 and 3 such that item 3 = 2 times size of item 2

however, if the width is defined for fles this may not happen. Therefore flex-basis is used


All the properties can be directly used in a single line as:

flex:    1      0       200px; 
  ->  (grow) (shrink)  (basis)  

most of the times, only grow is used