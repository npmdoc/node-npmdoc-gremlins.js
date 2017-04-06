# api documentation for  [gremlins.js (v0.1.0)](https://github.com/marmelab/gremlins.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-gremlins.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gremlins.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gremlins.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gremlins.js)
#### A monkey testing library written in JavaScript, for Node.js and the browser. Use it to check the robustness of web applications by unleashing a horde of undisciplined gremlins.

[![NPM](https://nodei.co/npm/gremlins.js.png?downloads=true)](https://www.npmjs.com/package/gremlins.js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gremlins.js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gremlins.js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gremlins.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gremlins.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gremlins.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Francois Zaninotto"
    },
    "bugs": {
        "url": "https://github.com/marmelab/gremlins.js/issues"
    },
    "dependencies": {},
    "description": "A monkey testing library written in JavaScript, for Node.js and the browser. Use it to check the robustness of web applications by unleashing a horde of undisciplined gremlins.",
    "devDependencies": {},
    "directories": {
        "example": "examples"
    },
    "dist": {
        "shasum": "8903d88710bedc8d18d0a1ddd48bfeca82a914cb",
        "tarball": "https://registry.npmjs.org/gremlins.js/-/gremlins.js-0.1.0.tgz"
    },
    "homepage": "https://github.com/marmelab/gremlins.js",
    "keywords": [
        "monkey",
        "test",
        "testing",
        "stress",
        "gremlin"
    ],
    "license": "MIT",
    "main": "gremlins.min.js",
    "maintainers": [
        {
            "name": "fzaninotto",
            "email": "fzaninotto@gmail.com"
        }
    ],
    "name": "gremlins.js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/marmelab/gremlins.js.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gremlins.js](#apidoc.module.gremlins.js)
1.  [function <span class="apidocSignatureSpan">gremlins.js.</span>createHorde ()](#apidoc.element.gremlins.js.createHorde)
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>js.mogwais
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>js.species
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>js.strategies
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>mogwais
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>species
1.  object <span class="apidocSignatureSpan">gremlins.js.</span>strategies

#### [module gremlins.js.mogwais](#apidoc.module.gremlins.js.mogwais)
1.  [function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>alert ()](#apidoc.element.gremlins.js.mogwais.alert)
1.  [function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>fps ()](#apidoc.element.gremlins.js.mogwais.fps)
1.  [function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>gizmo ()](#apidoc.element.gremlins.js.mogwais.gizmo)

#### [module gremlins.js.species](#apidoc.module.gremlins.js.species)
1.  [function <span class="apidocSignatureSpan">gremlins.js.species.</span>clicker ()](#apidoc.element.gremlins.js.species.clicker)
1.  [function <span class="apidocSignatureSpan">gremlins.js.species.</span>formFiller ()](#apidoc.element.gremlins.js.species.formFiller)
1.  [function <span class="apidocSignatureSpan">gremlins.js.species.</span>scroller ()](#apidoc.element.gremlins.js.species.scroller)
1.  [function <span class="apidocSignatureSpan">gremlins.js.species.</span>typer ()](#apidoc.element.gremlins.js.species.typer)

#### [module gremlins.js.strategies](#apidoc.module.gremlins.js.strategies)
1.  [function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>allTogether ()](#apidoc.element.gremlins.js.strategies.allTogether)
1.  [function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>bySpecies ()](#apidoc.element.gremlins.js.strategies.bySpecies)
1.  [function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>distribution ()](#apidoc.element.gremlins.js.strategies.distribution)



# <a name="apidoc.module.gremlins.js"></a>[module gremlins.js](#apidoc.module.gremlins.js)

#### <a name="apidoc.element.gremlins.js.createHorde"></a>[function <span class="apidocSignatureSpan">gremlins.js.</span>createHorde ()](#apidoc.element.gremlins.js.createHorde)
- description and source-code
```javascript
createHorde = function (){return new i}
```
- example usage
```shell
...
This practice, also known as [Monkey testing](http://en.wikipedia.org/wiki/Monkey_test), is very common in mobile application development
 (see for instance the [Android Monkey program](http://developer.android.com/tools/help/monkey.html)). Now that frontend (MV*, d3
.js, Backbone.js, Angular.js, etc.) and backend (Node.js) development use persistent JavaScript applications, this technique becomes
 valuable for web applications.

## Basic Usage

A gremlins *horde* is an army of specialized gremlins ready to mess up your application. *unleash* the gremlins to start the stress
 test:

'''js
var horde = gremlins.createHorde()
horde.unleash();
// gremlins will act randomly, at 10 ms interval, 100 times
'''

'gremlins.js' provides several gremlin *species*: some click everywhere on the page, others enter data in form inputs, others scroll
 the window in every possible direction, etc.

You will see traces of the gremlins actions on the screen (they leave red traces) and in the console log:
...
```



# <a name="apidoc.module.gremlins.js.mogwais"></a>[module gremlins.js.mogwais](#apidoc.module.gremlins.js.mogwais)

#### <a name="apidoc.element.gremlins.js.mogwais.alert"></a>[function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>alert ()](#apidoc.element.gremlins.js.mogwais.alert)
- description and source-code
```javascript
alert = function (){function l(){o.watchEvents.indexOf("alert")!==-1&&(window.alert=function(e){o.logger.warn("mogwai ","alert     ",e,"
alert")}),o.watchEvents.indexOf("confirm")!==-1&&(window.confirm=function(e){o.confirmResponse(),o.logger.warn("mogwai ","alert     ",
e,"confirm")}),o.watchEvents.indexOf("prompt")!==-1&&(window.prompt=function(e){o.promptResponse(),o.logger.warn("mogwai ","alert
     ",e,"prompt")})}var e=["alert","confirm","prompt"],r=function(){return o.randomizer.bool()},i=function(){return o.randomizer
.sentence()},s={warn:function(){}},o={watchEvents:e,confirmResponse:r,promptResponse:i,logger:s,randomizer:new n},u=window.alert
,a=window.confirm,f=window.prompt;return l.cleanUp=function(){return window.alert=u,window.confirm=a,window.prompt=f,l},t(l,o),l
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gremlins.js.mogwais.fps"></a>[function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>fps ()](#apidoc.element.gremlins.js.mogwais.fps)
- description and source-code
```javascript
fps = function (){function o(e){e-i>r.delay&&(u(e),i=e);if(!s)return;window.requestAnimationFrame(o)}function u(){function t(t){e=t,window
.requestAnimationFrame(n)}function n(t){var n=t-e<16?60:1e3/(t-e),i=r.levelSelector(n);r.logger[i]("mogwai ","fps       ",n)}var
 e;window.requestAnimationFrame(t)}function a(){s=!0,window.requestAnimationFrame(o)}var e={log:function(){},warn:function(){},error
:function(){}},n=function(e){return e<10?"error":e<20?"warn":"log"},r={delay:500,levelSelector:n,logger:e},i=-Infinity,s;return
a.cleanUp=function(){return s=!1,a},t(a,r),a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gremlins.js.mogwais.gizmo"></a>[function <span class="apidocSignatureSpan">gremlins.js.mogwais.</span>gizmo ()](#apidoc.element.gremlins.js.mogwais.gizmo)
- description and source-code
```javascript
gizmo = function (){function s(){function s(){e++,e==n.maxErrors&&(t.stop(),window.setTimeout(function(){n.logger.warn("mogwai ","gizmo     ","
stopped test execution after ",n.maxErrors,"errors")},4))}var e=0,t=this;r=window.onerror,window.onerror=function(e,t,n){return
s(),r?r(e,t,n):!1},i=n.logger.error,n.logger.error=function(){s(),i.apply(n.logger,arguments)}}var e={warn:function(){}},n={maxErrors
:10,logger:e},r,i;return s.cleanUp=function(){return window.onerror=r,n.logger.error=i.bind(n.logger),s},t(s,n),s}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gremlins.js.species"></a>[module gremlins.js.species](#apidoc.module.gremlins.js.species)

#### <a name="apidoc.element.gremlins.js.species.clicker"></a>[function <span class="apidocSignatureSpan">gremlins.js.species.</span>clicker ()](#apidoc.element.gremlins.js.species.clicker)
- description and source-code
```javascript
clicker = function (){function f(){var t,n,r,i,s=0;do{t=a.positionSelector(),n=t[0],r=t[1],i=e.elementFromPoint(n,r),s++;if(s>a.maxNbTries
)return!1}while(!i||!a.canClick(i));var o=e.createEvent("MouseEvents"),u=a.randomizer.pick(a.clickTypes);o.initMouseEvent(u,!0,!
0,window,0,0,0,0,0,!1,!1,!1,!1,0,null),i.dispatchEvent(o),typeof a.showAction=="function"&&a.showAction(n,r,u),typeof a.logger.log
=="function"&&a.logger.log("gremlin","clicker   ",u,"at",n,r)}var e=window.document,r=e.body,i=["click","click","click","click","
click","click","dblclick","dblclick","mousedown","mouseup","mouseover","mouseover","mouseover","mousemove","mouseout"],s=function
(){return[a.randomizer.natural({max:e.documentElement.clientWidth-1}),a.randomizer.natural({max:e.documentElement.clientHeight-1
})]},o=function(t,n){var i=e.createElement("div");i.style.border="3px solid red",i.style["border-radius"]="50%",i.style.width="40px
",i.style.height="40px",i.style["box-sizing"]="border-box",i.style.position="absolute",i.style.webkitTransition="opacity 1s ease
-out",i.style.mozTransition="opacity 1s ease-out",i.style.transition="opacity 1s ease-out",i.style.left=t-20+"px",i.style.top=n-
20+"px";var s=r.appendChild(i);setTimeout(function(){r.removeChild(s)},1e3),setTimeout(function(){s.style.opacity=0},50)},u=function
(){return!0},a={clickTypes:i,positionSelector:s,showAction:o,canClick:u,maxNbTries:10,logger:{},randomizer:new n};return t(f,a),
f}
```
- example usage
```shell
...
By default, all gremlins and mogwais species are added to the horde.

You can also choose to add only the gremlins species you want, using the 'gremlin()' function of the 'horde' object:

'''js
gremlins.createHorde()
  .gremlin(gremlins.species.formFiller())
  .gremlin(gremlins.species.clicker().clickTypes(['click']))
  .gremlin(gremlins.species.scroller())
  .gremlin(function() {
    window.$ = function() {};
  })
  .unleash();
'''
...
```

#### <a name="apidoc.element.gremlins.js.species.formFiller"></a>[function <span class="apidocSignatureSpan">gremlins.js.species.</span>formFiller ()](#apidoc.element.gremlins.js.species.formFiller)
- description and source-code
```javascript
formFiller = function (){function u(){var t=[],n=d();for(var r in o.elementMapTypes)o.elementMapTypes.hasOwnProperty(r)&&t.push(r);var i,s=0;
do{var u=e.querySelectorAll(t.join(","));if(u.length===0)return!1;i=o.randomizer.pick(u),s++;if(s>o.maxNbTries)return!1}while(!i
||!o.canFillElement(i));var a=null;for(var f in o.elementMapTypes)if(i[n](f)){a=f;break}var l=o.elementMapTypes[a](i);typeof o.showAction
=="function"&&o.showAction(i),typeof o.logger.log=="function"&&o.logger.log("gremlin","formFiller","input",l,"in",i)}function a(
e){var t=o.randomizer.character();return e.value+=t,t}function f(e){var t=o.randomizer.character({pool:"0123456789"});return e.value
+=t,t}function l(e){var t=e.querySelectorAll("option"),n=o.randomizer.pick(t);for(var r=0,i=t.length;r<i;r++){var s=t[r];s.selected
=s.value==n.value}return n.value}function c(t){var n=e.createEvent("MouseEvents");return n.initMouseEvent("click",!0,!0,window,0
,0,0,0,0,!1,!1,!1,!1,0,null),t.dispatchEvent(n),t.value}function h(t){var n=e.createEvent("MouseEvents");return n.initMouseEvent
("click",!0,!0,window,0,0,0,0,0,!1,!1,!1,!1,0,null),t.dispatchEvent(n),t.value}function p(e){var t=o.randomizer.email();return e
.value=t,t}function d(){var t=e.querySelector("body");return(t.mozMatchesSelector||t.msMatchesSelector||t.oMatchesSelector||t.webkitMatchesSelector
).name}var e=window.document,r={'input[type="text"]':a,'input[type="password"]':a,'input[type="number"]':f,select:l,'input[type="
radio"]':c,'input[type="checkbox"]':h,'input[type="email"]':p,"input:not([type])":a},i=function(e){typeof e.attributes["data-old
-border"]=="undefined"&&(e.attributes["data-old-border"]=e.style.border);var t=e.attributes["data-old-border"];e.style.border="1px
 solid red",setTimeout(function(){e.style.border=t},500)},s=function(){return!0},o={elementMapTypes:r,showAction:i,canFillElement
:s,maxNbTries:10,logger:{},randomizer:new n};return t(u,o),u}
```
- example usage
```shell
...

By default, all gremlins and mogwais species are added to the horde.

You can also choose to add only the gremlins species you want, using the 'gremlin()' function of the 'horde' object:

'''js
gremlins.createHorde()
  .gremlin(gremlins.species.formFiller())
  .gremlin(gremlins.species.clicker().clickTypes(['click']))
  .gremlin(gremlins.species.scroller())
  .gremlin(function() {
    window.$ = function() {};
  })
  .unleash();
'''
...
```

#### <a name="apidoc.element.gremlins.js.species.scroller"></a>[function <span class="apidocSignatureSpan">gremlins.js.species.</span>scroller ()](#apidoc.element.gremlins.js.species.scroller)
- description and source-code
```javascript
scroller = function (){function a(){var e=u.positionSelector(),t=e[0],n=e[1];window.scrollTo(t,n),typeof u.showAction=="function"&&u.showAction
(t,n),typeof u.logger.log=="function"&&u.logger.log("gremlin","scroller  ","scroll to",t,n)}var e=window.document,r=e.documentElement
,i=e.body,s=function(){var e=Math.max(i.scrollWidth,i.offsetWidth,r.scrollWidth,r.offsetWidth,r.clientWidth),t=Math.max(i.scrollHeight
,i.offsetHeight,r.scrollHeight,r.offsetHeight,r.clientHeight);return[u.randomizer.natural({max:e-r.clientWidth}),u.randomizer.natural
({max:t-r.clientHeight})]},o=function(t,n){var s=e.createElement("div");s.style.border="3px solid red",s.style.width=r.clientWidth
-25+"px",s.style.height=r.clientHeight-25+"px",s.style.position="absolute",s.style.webkitTransition="opacity 1s ease-out",s.style
.mozTransition="opacity 1s ease-out",s.style.transition="opacity 1s ease-out",s.style.left=t+10+"px",s.style.top=n+10+"px";var o
=i.appendChild(s);setTimeout(function(){i.removeChild(o)},1e3),setTimeout(function(){o.style.opacity=0},50)},u={positionSelector
:s,showAction:o,logger:{},randomizer:new n};return t(a,u),a}
```
- example usage
```shell
...

You can also choose to add only the gremlins species you want, using the 'gremlin()' function of the 'horde' object:

'''js
gremlins.createHorde()
  .gremlin(gremlins.species.formFiller())
  .gremlin(gremlins.species.clicker().clickTypes(['click']))
  .gremlin(gremlins.species.scroller())
  .gremlin(function() {
    window.$ = function() {};
  })
  .unleash();
'''

If you just want to add your own gremlins in addition to the default ones, use the 'allGremlins()' function:
...
```

#### <a name="apidoc.element.gremlins.js.species.typer"></a>[function <span class="apidocSignatureSpan">gremlins.js.species.</span>typer ()](#apidoc.element.gremlins.js.species.typer)
- description and source-code
```javascript
typer = function (){function a(){var t=Math.max(i.scrollWidth,i.offsetWidth,r.scrollWidth,r.offsetWidth,r.clientWidth),n=Math.max(i.scrollHeight
,i.offsetHeight,r.scrollHeight,r.offsetHeight,r.clientHeight),s=e.createEvent("KeyboardEvent"),o=typeof s.initKeyboardEvent!="undefined
"?"initKeyboardEvent":"initKeyEvent",a=u.randomizer.natural({max:360}),f=u.randomizer.natural({max:r.clientWidth-1}),l=u.randomizer
.natural({max:r.clientHeight-1}),c=e.elementFromPoint(f,l);s[o](u.randomizer.pick(u.eventTypes),!0,!0,c,!1,!1,!1,!1,a,0),c.dispatchEvent
(s),typeof u.showAction=="function"&&u.showAction(c,f,l,a),typeof u.logger.log=="function"&&u.logger.log("gremlin","typer
type",a,"at",f,l)}var e=window.document,r=e.documentElement,i=e.body,s=["keypress","keyup","keydown"],o=function(t,n,r,s){var o=
e.createElement("div");o.style.border="3px solid orange",o.style["border-radius"]="50%",o.style.width="40px",o.style.height="40px
",o.style["box-sizing"]="border-box",o.style.position="absolute",o.style.webkitTransition="opacity 1s ease-out",o.style.mozTransition
="opacity 1s ease-out",o.style.transition="opacity 1s ease-out",o.style.left=n+"px",o.style.top=r+"px",o.style.textAlign="center
",o.style.paddingTop="7px",o.innerHTML=String.fromCharCode(s);var u=i.appendChild(o);setTimeout(function(){i.removeChild(u)},1e3
),setTimeout(function(){u.style.opacity=0},50)},u={eventTypes:s,showAction:o,logger:{},randomizer:new n};return t(a,u),a}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gremlins.js.strategies"></a>[module gremlins.js.strategies](#apidoc.module.gremlins.js.strategies)

#### <a name="apidoc.element.gremlins.js.strategies.allTogether"></a>[function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>allTogether ()](#apidoc.element.gremlins.js.strategies.allTogether)
- description and source-code
```javascript
allTogether = function (){function s(n,s,u){function l(e){t(n,[],f,e)}function c(t){if(r)return;if(t>=a)return o();l(function(){setTimeout(function
(){c(++t)},e.delay)})}var a=s&&s.nb?s.nb:e.nb,f=this;r=!1,i=u,c(0)}function o(){typeof i=="function"&&i(),i=null}var e={delay:10
,nb:100},r,i;return s.stop=function(){r=!0,setTimeout(o,4)},n(s,e),s}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gremlins.js.strategies.bySpecies"></a>[function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>bySpecies ()](#apidoc.element.gremlins.js.strategies.bySpecies)
- description and source-code
```javascript
bySpecies = function (){function s(n,s,u){function l(n,i,s){if(r)return;if(i>=a)return s();t([n],[],f,function(){setTimeout(function(){l(n,++
i,s)},e.delay)})}function c(){if(r)return;if(n.length===0)return o();l(n.shift(),0,c)}var a=s&&s.nb?s.nb:e.nb,n=n.slice(0),f=this
;r=!1,i=u,c()}function o(){typeof i=="function"&&i(),i=null}var e={delay:10,nb:100},r,i;return s.stop=function(){r=!0,setTimeout
(o,4)},n(s,e),s}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gremlins.js.strategies.distribution"></a>[function <span class="apidocSignatureSpan">gremlins.js.strategies.</span>distribution ()](#apidoc.element.gremlins.js.strategies.distribution)
- description and source-code
```javascript
distribution = function (){function o(n,r,o){function p(r,s,o){if(i)return;if(s>=l)return f();t([r],[],h,function(){setTimeout(function(){p(a(n
,c),++s,o)},e.delay)})}var l=r&&r.nb?r.nb:e.nb,n=n.slice(0),c=e.distribution.length===0?u(n):e.distribution,h=this;if(l===0)return
 o();i=!1,s=o,p(a(n,c),0,p)}function u(e){var t=e.length;if(t===0)return[];var n=[],r=1/t;for(var i=0;i<t;i++)n.push(r);return n
}function a(t,n){var r=0,i=e.randomizer.floating({min:0,max:1});for(var s=0,o=t.length;s<o;s++){r+=n[s];if(i<=r)return t[s]}return
 function(){}}function f(){typeof s=="function"&&s(),s=null}var e={distribution:[],delay:10,nb:100,randomizer:new r},i,s;return
o.stop=function(){i=!0,setTimeout(f,4)},n(o,e),o}
```
- example usage
```shell
...
'''

### Setting Up a Strategy

By default, gremlins will attack in random order, in a uniform distribution, separated by a delay of 10ms. This attack strategy
is called the [distribution](src/strategies/distribution.js) strategy. You can customize it using the 'horde.strategy()' method:

'''js
horde.strategy(gremlins.strategies.distribution()
  .delay(50) // wait 50 ms between each action
  .distribution([0.3, 0.3, 0.3, 0.1]) // the first three gremlins have more chances to be executed than the last
)
'''

You can also use another strategy. A strategy is just a callback expecting three parameters: an array of gremlins, a parameter object
 (the one passed to 'unleash()'), and a final callback. Two other strategies are bundled ([allTogether](src/strategies/allTogether
.js) and [bySpecies](src/strategies/bySpecies.js)), and it should be fairly easy to implement a custom strategy for more sophisticated
 attack scenarios.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
