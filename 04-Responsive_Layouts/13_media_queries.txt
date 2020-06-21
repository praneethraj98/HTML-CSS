Testing of media queries through Google dev tools (ctrl + shift + i) and test on various devices

Set max and min widths for various devices (phones, tablets and PCs) by checking their heights on Goolge dev tools

only screen - only applies to screen

- can have seperate files for media queries
 eg:   <link rel="stylesheet" media="screen and (max-width: 768px)" href="mobile.css">
    media attribute makes sure this stylesheet is opened only if screen is <= 768px
- always have media queries link after main stylesheet