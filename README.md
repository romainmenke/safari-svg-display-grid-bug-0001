# safari-svg-display-grid-bug-0001

## Update 2022-04-26

This seems unrelated to `display: grid;`,  
the simplest reproduction I've currently found is adding some plain text before an SVG.

compare:
- https://romainmenke.github.io/safari-svg-display-grid-bug-0001/svg-with-text.html
- https://romainmenke.github.io/safari-svg-display-grid-bug-0001/svg-without-text.html

## Original report

I expect all squares to be of equal size (16x16)

In reality `display: grid;` seems to cause some SVG's to alter size.

Test in Safari 16.4

<img width="1009" alt="Screenshot 2023-04-25 at 18 21 06" src="https://user-images.githubusercontent.com/11521496/234340479-08cab89e-90b4-4626-9d1f-f2613490a398.png">

bug report : https://bugs.webkit.org/show_bug.cgi?id=255929
