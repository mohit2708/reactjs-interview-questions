https://codesandbox.io/  -> online react run

## React Install
* Install NodeJs (https://nodejs.org/en/download/) And Npm  // jab node install karte hai to automatically npm install ho jata hai<br>
  * __Check node install__:-  node -v
  * __Check npm install__:- npm -v



* Install Visual studio/sublime/atom/Brackets
* Install React from Terminal<br>
  -> npx create-react-app <project-name> <br>
  -> cd my-app <br>
  -> npm start <br>


## without import react only write pure javascript in babel js in index.js
```php
var h1 = document.createElement("h1");
h1.innerHTML = "Mohit Saxena";
document.getElementById("root").appendChild(h1);
```

### Multiple Elements inside ReactDOM.render()
```php
ReactDOM.render(
<React.Fragment>  
  <Heading/>
  <h6>my name is {fname} </h6>
 </React.Fragment>
  ,
  document.getElementById('root')
);
```
__(OR)__
```php
ReactDOM.render(
<>  
  <Heading/>
  <h6>my name is {fname} </h6>
 </>
  ,
  document.getElementById('root')
);
```
__(OR)__
```php
ReactDOM.render(
[  
  <Heading/>,
  <h6>my name is {fname} </h6>,
]
  ,
  document.getElementById('root')
);
```
### Javascript Expression
```php
const fname = "mohit";
const lname = "saxena";
const currdate = new Date().toLocaleDateString();
const currtime = new Date().toLocaleTimeString();
const heading = {
  color : '#f66666',
  textTransformation : 'capitalize',
  fontWeight : 'bold'
};
ReactDOM.render( 
<>
<h1>My Name is {fname}</h1>
<h1 className="heading" style={heading}>Hello</h1> // class ki jaghe className use hota hai
<p>add {2+3} </p>
<p>Math Randam {Math.random()}</p>
<p>My Name is {fname + " " + lname} {lname}</p>
<h1>My Name is {`${fname} ${lname}`}</h1>
<p>current date is {currdate}</p>
<p>current time is {currtime}</p>
</>,
  document.getElementById('root')
);

```

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




