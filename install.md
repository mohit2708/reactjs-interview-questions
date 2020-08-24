https://codesandbox.io/  -> online react run

## React Install
* Install NodeJs (https://nodejs.org/en/download/) And Npm  // jab node install karte hai to automatically npm install ho jata hai<br>
__Check node install__ 
```php
-> node -v
```
__Check npm install__
-> npm -v
```


* Install Visual studio/sublime/atom/Brackets
* Install React from Terminal<br>
  -> npx create-react-app <project-name> <br>
  -> cd my-app <br>
  -> npm start <br>



## Ques. What are React Components?
React components are independent and reusable code.


### Types of React Components?
* __Functional Components__
```php
function Title()
{
    return <h1>I am Title</h1>;
}
```

* __Class Components__
```php
class Title extends React.Component
{
    render(){
          return <h1>I am Title</h1>;
    }
}
```

* Pure Components
* Higher-Order Components


### Go to Folder -> Src -> index.js
```php
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';


import App from './App';
import * as serviceWorker from './serviceWorker';

ReactDOM.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById('root')
);

// If you want your app to work offline and load faster, you can change
// unregister() to register() below. Note this comes with some pitfalls.
// Learn more about service workers: https://bit.ly/CRA-PWA
serviceWorker.unregister();
```

### Go to Folder -> Src -> app.js
```php
import React from 'react';
import logo from './logo.svg';
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className="App-link"
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Learn React
        </a>
      </header>
    </div>
  );
}

export default App;
```




