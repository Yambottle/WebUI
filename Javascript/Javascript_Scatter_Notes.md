# Javascript Scatter Notes

## Javascript Array
## 1. Define
```
var a = new Array(); | var a[];
var a = new Array(length); | none;
var a = new Array(e1, e2, e3...); | var a[e1, e2, e3...];
```

## 2. Index
Only positive integer(n >= 0) can be index, others(string, n < 0) will be treated as attribute

## 3. Length
* Non fixed: like vector, length = maximum index + 1
* Fixed: drop bound overflow

## 4. Add/Delete/Insert
* Index: delete a[2]; //set undefine
* Stack: push()/pop() //length changed
* Queue: push()/shift()/unshift() //length changed
* Add, delete, insert: splice(start, end, e1, e2, e3...) //length changed

## 5. Util Method
* join(char): like toString()
* slice(start, end): [start, end) end could be negative
* concat(array)
* reverse(): reverse order
* sort(cmp): cmp - alphabetic by default

## Others

##### 1. Undefined vs Null
* undefined: used when defined but without init
* null: used when manually clear a variable

##### 2. Using "new" to specify data type(ObjectClass)

##### 3. Auto put variable into lobal if it's without declearation

##### 4. "===" equal value and type

##### 5. label: code -> goto
* break label;
* continue label

##### 6. With HTML/CSS DOM
* document.getElementById(id).innerHTML
* document.getElementById(id).attribute
* document.getElementById(id).style.property
* document.getElementById(id).onclick
* onload/onunload: enter/leave page
* onchange: input
* onmouseover/onmouseout
* onmousedown->onmouseup->onclick

##### 7. DOM Method
* appendChild()
* emoveChild()
* replaceChild()
* insertBefore()
* createAttribute()
* createElement()
* createTextNode()
* getAttribute()
* setAttribute()

##### 8. DOM element access
```
//list and index
var x=document.getElementsByTagName("p");
y=x[0];

//length for a loop
length = x.length

// parent or child
x.parentNode
x.firstChild
x.lastChild
x.childNodes[0]

//document or body
document.documentElement
document.body
```

##### 9. Object
* attribute
* function: function has to be decleared as attribute:
```
function person(name,age){
    this.name = name;
    this.age = age;
    this.changeName=changeName;// function declearation
    function changeName(name){
        this.lastname=name;
    }
}
```

##### 10. Number variable
* 15(<16) saftey digits integer
* 17 floating point
* inaccurate floating point calculation

##### 11. Boolean
```
//All in false
var myBoolean=new Boolean();
var myBoolean=new Boolean(0);
var myBoolean=new Boolean(null);
var myBoolean=new Boolean("");
var myBoolean=new Boolean(false);
var myBoolean=new Boolean(NaN);

//All in true
var myBoolean=new Boolean(1);
var myBoolean=new Boolean(true);
var myBoolean=new Boolean("true");
var myBoolean=new Boolean("false");
var myBoolean=new Boolean("Bill Gates");
```

##### 12. RegExp
* boolean test()
* String exec()

##### 13. Window.location
* location.attribute: path, port, url(href, pathname)
* location.assign(): redirect

##### 14. Window.navigator
* navigator.attribute: browser info
* However, when detecting type of browser, it could be changed by user. Instead, using different supported Object to detect browser

##### 15. document.cookie
A string: "cname=cvalue;" + expire

