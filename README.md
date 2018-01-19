# splitType
split type is split.js wapper

### status
___=>fix___ is spec fix.
___=>comp___ is complete the spec.

### splitType.js draft
- package name is splitType.js
- open funciton is one. splitType({type:__str__,el: element },{opt}); return element.   
if element is not, write the document.body
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
 2. usage image. split.js is already exist tareget element on the HTML.
```
var fullbox = document.getElm..Id
splitType({type:'lr',el:fullbox});
//or
splitType({type:'lrtbc',el:fullbox},{l:'20%',r:'80%',t:'20%',c:'60%',b:'20%'}); //default size
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
