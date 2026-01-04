# PowerBI

```dax
Milestone SVG = 
VAR barWidth = 80
VAR progressWidth = barWidth * [Progress %]

RETURN
"data:image/svg+xml;utf8,
<svg xmlns='http://www.w3.org/2000/svg'>
  <rect x='10' y='5' width='" & barWidth & "' height='10' rx='5' fill='lightgrey' />
  <rect x='10' y='5' width='" & progressWidth & "' height='10' rx='5' fill='green' />
</svg>"
