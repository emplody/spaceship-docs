# &#x201C;Fetch&#x201D; Methods

## asyncState(value)

<p><a href="https://github.com/emplody/spaceship/tree/develop/utils/spaceship.asyncState">source</a> <a href="https://www.npmjs.com/package/@emplodies/spaceship.async-state">npm package</a></p>
<p>Easily manage status that pending, success, failure at <code>asynchronous request</code>.

<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>value</code> <em>(string)</em>: The fetchState what you handle.</li>
<h4>Returns</h4>
<p><em>(Object)</em>: Returns the fetchState.</p>
<h4>Example</h4>

```js
import asyncState, { PENDING, SUCCESS, FAILURE } from "./index.js";

class Example {
  constructor() {
    this.myFetchStatus = asyncState();
    // myFetchStatus
    // {
    //   pending: false,
    //   success: false,
    //   failure: false,
    // }
  }

  getData() {
    this.myFetchStatus = asyncState(PENDING);
    // myFetchStatus
    // {
    //   pending: true,
    //   success: false,
    //   failure: false,
    // }
    fetch("http://test/data")
      .then(res => {
        this.myFetchStatus = asyncState(SUCCESS);
        // myFetchStatus
        // {
        //   pending: false,
        //   success: true,
        //   failure: false,
        // }
        return res.json();
      })
      .catch(err => {
        this.myFetchStatus = asyncState(FAILURE);
      });
  }

  renderExample() {
    const { myFetchStatus } = this;
    const el = document.getElementById("example");

    if (myFetchStatus.PENDING) {
      return (el.innerHTML = "Please wait...");
    }
    if (myFetchStatus.SUCCESS) {
      return (el.innerHTML = "Data request successful!");
    }
    if (myFetchStatus.FAILURE) {
      return (el.innerHTML = "Data request failure 😥");
    }
  }
}
```

<hr>

## scriptLoader(src)

<p><a href="https://github.com/emplody/spaceship/tree/develop/utils/spaceship.scriptLoader">source</a> <a href="https://www.npmjs.com/package/@emplodies/spaceship.script-loader">npm package</a></p>
<p>When we want to <code>dynamically import</code> scripts.
</p>
<h4>Since</h4>
<p>1.0.0</p>
<h4>Arguments</h4>
<ol>
<li><code>src</code> <em>(string)</em>: The script what you want to import.</li>
</ol>
<h4>Returns</h4>
<p><em>(Promise)</em>: Returns the Promise with resolve, error function.</p>
<h4>Example</h4>

```js
function loadReact() {
  scriptLoader("https://unpkg.com/react-dom@16/umd/react-dom.development.js")
    .then(() => {
      const domContainer = document.querySelector("#like_button_container");
      ReactDOM.render(e(LikeButton), domContainer);
    })
    .catch(err => console.err(err));
}
```
