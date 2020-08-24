## React Install
* Install NodeJs (https://nodejs.org/en/download/) And Npm 
* Install Visual studio/sublime/atom/Brackets
* Install React from Terminal<br>
  -> npx create-react-app <project-name> <br>
  -> cd my-app <br>
  -> npm start <br>

## Check node install
-> node -v

## check npm install
-> npm -v


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
