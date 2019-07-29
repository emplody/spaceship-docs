# &#x201C;Data&#x201D; Methods

## getPadNumber(count, value)

<p><a href="https://github.com/lodash/lodash/blob/4.17.11/lodash.js#L6841">source</a> <a href="https://www.npmjs.com/package/lodash.chunk">npm package</a></p>
<p>geFormattedNumberString What you want.</p>
<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>count</code> <em>(number)</em>: The Number of digits</li>
<li><code>value</code> <em>(number)</em>: The number(value) what you want to format.</li>
</ol>
<h4>Returns</h4>
<p><em>(string)</em>: Returns formatted number.</p>
<h4>Example</h4>

```js
getPadNumber(3, 1);
// => "001"
getPadNumber(2, 1);
// => "01"
```

<hr>

## normalizeKeyword(keyword)

// TODO: (sk) : add Description

<p><a href="https://github.com/lodash/lodash/blob/4.17.11/lodash.js#L6841">source</a> <a href="https://www.npmjs.com/package/lodash.chunk">npm package</a></p>
<p>Creates an array of elements split into groups the length of <code>size</code>.
If <code>array</code> can&apos;t be split evenly, the final chunk will be the remaining
elements.</p>
<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>keyword = ''</code> <em>(string)</em>: The value to process.</li>
</ol>
<h4>Returns</h4>
<p><em>(string)</em>: Returns the new string.</p>
<h4>Example</h4>

```js
normalizeKeyword("ㄴ네이버ㅓ");
// => '네이버'
normalizeKeyword("미국ㄱ");
// => '미국'
```

<hr>

## objToParams(obj)

<p><a href="https://github.com/emplody/spaceship/tree/develop/utils/spaceship.objToParams">source</a> <a href="https://www.npmjs.com/package/@emplodies/spaceship.obj-to-params">npm package</a></p>
<p>Make url with <code>parameters</code> from object data.
</p>
<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>obj</code> <em>(Object)</em>: The Object to process.</li>
</ol>
<h4>Returns</h4>
<p><em>(string)</em>: Returns the url with query string .</p>
<h4>Example</h4>

```js
objToParams({ job: "programmer" });
// => 'job=programmer'

objToParams({ name: "abel", age: 23, gender: "male" });
// => 'name=abel&age=23&gender=male'
```

<hr>

## paramsToObj()

<p><a href="https://github.com/lodash/lodash/blob/4.17.11/lodash.js#L6841">source</a> <a href="https://www.npmjs.com/package/lodash.chunk">npm package</a></p>
<p>Get data params and change to <code>object.</code></p>

<h4>Since</h4>
<p>1.0.0</p>
<h4>Returns</h4>
<p><em>(Object)</em>: Returns the new object from query parameters.</p>
<h4>Example</h4>

```js
//  url: 'https://www.example.com?test=true'
paramsToObj();
// => { test: 'true' }
```

<hr>

## toTimeString(timestamp, separator = ':')

<p><a href="https://github.com/lodash/lodash/blob/4.17.11/lodash.js#L6841">source</a> <a href="https://www.npmjs.com/package/lodash.chunk">npm package</a></p>
<p>get <code>Formmated TimeStamp</code> from system time stamp.</p>

<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>timestamp</code> <em>(string)</em>: The system timestamp.</li>
</ol>
<li><code>separator</code> <em>(string)</em>: The separator between timestamp.</li>
</ol>
<h4>Returns</h4>
<p><em>(string)</em>: Returns the formatted timestamp.</p>
<h4>Example</h4>

```js
// TODO: (SY) : Refactor ..
```
