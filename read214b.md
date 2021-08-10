# Transforms: 
1. The transform property comes in two different settings, two-dimensional and three-dimensiona.
2. syntax:

`selector {`

  `-transform: property (value);`

`}`

3. transform Properties:
* 3D,2D Rotate.
* 3D,2D Scale
* 3D,2D Translate
* 3D,2D Skew.

# Transition and Animations: 
* Transitions provide a change from one state to another.

* animations can set multiple points of transition upon different keyframes.

* determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes..

* not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike.

* nimations can only apply a transition within a single property, not from one property to another.

* To set multiple points at which an element should undergo a transition, use the @keyframes rule.

* Simple CSS3 Transitions:
 
   1. Fade in: 

   `.fade{`

       ` opacity:0.5;`

`}`

`.fade:hover {`

`opacity:1;`

`}`

2. Change color: 

`.color:hover{`

`background:#53a7ea;`

`}`

3. Grow & Shrink: 

`grow:hover{`

`-webkit-transform: scale(1.3);`

 `-ms-transform: scale(1.3);`

   ` transform: scale(1.3);`

`}`

4. 3D shadow:

`.threed:hover {`

`box-shadow:`

`1px 1px #53a7ea,`

`2px 2px #53a7ea,`

` 3px 3px #53a7ea;`

`-webkit-transform: translateX (-3px);`

`transform: translateX(-3px);`

`}`

![g](https://coursework.vschool.io/content/images/2016/08/transition_example2.png)