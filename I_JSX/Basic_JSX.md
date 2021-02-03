# BASIC JSX
- Syntax extension for java script
- JSX is similat HTML but stored in the javascript files

### Elements
- Basic unit of JSX is called a JSX element
    ```
    <h1>Hello World</>
    ```
### JSX Elements Surroundings
As JSX can go everywhere as javascript element .
Example - 
-   JSX element being save as a js variable
    ```
    const myName = <h1>Biplaba Samantaray</h1>
    ```
-   JSX element being save as a js varible
    ```
    const myDetails = 
    {
        name : <p>Biplaba Samantaray</p>
        place : <p>Hyderabad</p>
        Employment type: <p>Intern</p>
    }
    ```
### Attributes
-   JSX elements have attributes as similar to the HTML
    Example -
    ```
    const p1 = <p id  = "large">foo</p>
    const p2 = <p id = "small">bar</p>
    ```
### Nested JSX
- Similar to HTML ,We can nested up jsx elements
    Example
    ```
    <a href = "https://www.biplabas.com">
        <p>Biplaba Samantaray's Portfolio</p>
    </a>
    // After wrapping up
    var myDiv = ( <div>
        <h1>Hello World</h1>
        </div> ) ;
    ```
### JSX Outer Elements
Outer element should limit to one .
| Right Way | Wrong Way |
| ------ | ------ |
|  var myDiv = ( <div> <h1>Hello</h1> <h1>World</h1> </div> ) ; | var myDiv = ( <h1>Hello</h1> <h1>World</h1> ) ; |
### Rendering JSX 
```
import React from 'react';
import ReactDOM from 'react-dom';
ReactDOM.render(<h1>Render me!</h1>,
                document.getElementById('app'))
```