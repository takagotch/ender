### ender
---
https://enderjs.com/

https://github.com/ender-js/Ender

```sh
ender build domready qwery underscore

ender build backbone
ender add domready qwery
ender remove qwery

npm instal ender -g
ender build scriptjs backbone@0.1.0 ../../myLocalPackage

ender add scriptjs

ender set foo@0.0.1
ender add scriptjs@0.1.0
ender remove domready

ender refresh
ender compile ./header.js ./footer.js ./my/app.js
ender info
ender search underscore
ender

ender build fee fie foe fum --output foobar --use yeehaw --max 10 \
--sandbox foo bar --silent --help --debug --externs what tha \
--client-lib BOOM --quiet --force-install --minifier none 
```

```js
$('#content a.button')
  .bind('click.button', function (e) {
    $(this).data('clicked', true).unbind()
    e.preventDefault()
  })
  .css({
      opacity: 1
    , color: 'red'
  })
  .fadeOut(250)
  
$.map(['a', 'b', 'c'], function (letter) {
  return letter.toUpperCase()
})

$.ajax('/data', function (resp) {
  $('#content').html(resp)
})


var _ = require('underscore')
_.each([1, 2, 3], alert)

$.ready(function () {
  $([1, 2, null, 3])
    .filter(function (item) { return item })
    .each(alert)
})

var myPackage = require('myPackage')

var _ = require('underscore')

var backbone = require('backbone')
  , _ = require('underscore')
  
backbone.Module(...)
_.each(...)

$.baz()
$.ender({ baz: require('foo').baz });
require('baz').baz()

provider("myPackage", myPackageObj)
provider('underscore', _)

$.ender({
  myUtility: myLibFn
})

$.myUtility()


$.ender({
  rand: function () {
    return this[Math.floor(Math.random() * this.length)]
  }
}, true)
$('p').read()

$._select = mySelectorEngine
$('#foo .bar')

$._select = function (selector, root) {
  return (root || document).querySelectorAll(selector)
})

$.domReady(function () {...})

$('#boosh a[rel~="bookmark"]').each(function (el) { ... })

$('#boosh p a[rel~="bookmark"]').hide().html('hello').css({
  color: 'red',
  'text-decoration': 'none'
}).addClass('blamo').after('x').show();

$('#content a').bind('keydown input', handler)
$('#content a').emit('customEvent')
$('#content a').remove('click.myClick')
```

```
{
  "name": "blamo",
  "description": "a thigs that blams the o's",
  "version": "1.0.0",
  "keywords": ["blamo", "ender"],
  "homepage": "http://example.com",
  "authors": ["Mr.Blam", "Miss O"],
  "repository": {
    "type": "*"
    "url": "https://github.com/fake-account/blamo.git"
  },
  "dependencies": {
    "klass": "*"
  },
  "main": "./src/project/blamo.js",
  "ender": "./src/exports/ender.js"
}
```


