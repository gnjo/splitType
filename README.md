# splitType
split type is split.js wapper

### status
___=>fix___ is spec fix.
___=>comp___ is complete the spec.

### splitType.js draft
- package name is splitType.js
- open funciton is one. splitType(str,{opt}); return element.
 1. str is type pattern.  lrtbc mix. left,right,top,bottom,center,vertical: v and vv,holizontal: h and hh.
```
lr is  l r and v
tb is  t b and h
tlr is t l r and v h
blr is b l r and v h
ltb is l t b and v h
rtb is r t b and v h
lrtb is l r t b and v vv h
lrtbc is l r t b c and v vv h hh
```
 2. usage image
```
var draw = document.body;
var box =splitType('lr');
box.id='testbox';
draw.appendChild(box);
//or
var fullbox =splitType('lrtbc',{l:'20%',r:'80%',t:'20%',c:'60%',b:'20%'}); //default size
fullbox.id= ....
....
//split panel access
fullbox.querySelector('.l');  
fullbox.querySelector('.r'); 
... t,c,b 
```
3. include image __=>fix__
```
<script src="//gnjo.github.io/splitType.js"></script>
<link rel="stylesheet" href="//gnjo.github.io/splitType.css">
```
