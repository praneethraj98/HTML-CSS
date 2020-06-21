practical use of After field is when you want to asterisk some labels of the form as compulsary

A seperate class (is-required) is formed for these specific labels, and then its styled in the css
content: '*' -> * appears next to the label. but is not part of the text


before and after are also used for overlays
Without before, if opacity is added, both the image as well as the text are made transparent

in order to just make the image transparent, before pseudo selector is used:
   header::before {
      content: '';
      background: url('https://source.unsplash.com/user/erondu/1600x900') no-repeat center center/cover;
      opacity: 0.2;
      position: absolute;
      top: 0;                     -> starts at the top
      left: 0;                    -> starts at the left
      width: 100%;                -> fills the entire width
      height: 100%;               -> fills the entire height
      z-index: -1;                -> sending it back
    }