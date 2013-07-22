#W3C WindowBase64#

Provides the **WindowBase64** interface defined in the "**Base64 utility methods**" (**HTML5 section 6.2**)

The **atob()** and **btoa()** methods allow authors to transform content to and from the base64 encoding.

In these APIs, for mnemonic purposes, the "b" can be considered to stand for "binary", and the "a" for "ASCII". In practice, though, **for primarily historical reasons, both the input and output of these functions are Unicode strings.**

##Requirements##

This polyfill will provide HTML5 compliant base64 interface to JavaScript platforms supporting the **Buffer API**.

It is currently supported by **node.js** and **Wakanda**.

Let me know if you are aware of other compatible platforms


##How to use##

You might use it directly from the module itself or apply it to any other object

ex:
```javascript
// Implements the WindowBase64 on the global object
require('w3c-windowbase64').WindowBase64.apply(this);
```
and then use it from whatever objects you want including the global object

```javascript
var base64Str = btoa('string to encode');
```



##Reference##
http://www.w3.org/TR/html5/webappapis.html#atob


## License (MIT License) ##

Copyright (c) 2013 Alexandre Morgaut

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
