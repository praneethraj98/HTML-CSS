Using div p {} in the style tag will style all the paragraphs inside the div

To Style only the direct childs of the div we use:
      div > p
The p tag inside the li is not styled because its a direct child of li and not p

To target the item directly after the div ends we use:
      div + p
This will style the immediate paragraphs after the div ends

To style based on attribute we use:
     a[target] {}
i,e. all the a tags with target attribute are styled

To style based on the value of the attribute
    a[target = '_blank'] {}

    input[type = 'text'],
    input[type = 'email'] {}