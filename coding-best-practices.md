
# Coding Best Practices

## Javascript & React Patterns

In order to write quality JavaScript code (rather ems6) code, you will have to master below code best practices intuitively:
- useRef
- implicit return of arrow functions const p = x => 1+x;
- the spread operator: ...Array
- conditional statements
- useEffect
- be able to: map over Arrays
- be able to: make anything into a custom component
- be able to: use useContext
- be able to: make custom hooks
- be able to: map over Objects with Object.keys(...)...
- use absolute imports
- Golden rule of coding: DRY - DO NOT REPEAT YOURSELF

### Examples: 

Understand conditional-statements like:
```
const [x,setX] = useState(null)

if(x) {
 ...
}

if(!!x) {
 ...
}

return (<div> 
  {x && ...}
</div>)

return (<div> 
  {!!x && ...}
</div>)
```

Understand useEffect [source](https://youtu.be/dpw9EHDh2bM?t=720)

Understand Custom Hooks [source](https://youtu.be/dpw9EHDh2bM?t=720)

Understand "usePrevious"-hook [source](https://blog.logrocket.com/how-to-get-previous-props-state-with-react-hooks/)

Map over an array
```
[1,2,3].map( x => <div>{x} </div>)
or 
return (<div> {persons.map(x => <Component name={x.name} sirname={x.sirname} > </Component>)}</div>)
```

Map over the keys of an object
- It is pretty much the same as mapping over an array, you just need to get the keys first.
```
Object.keys(obj).map(...) - 
```

Create useContext inside a ContextName.js file, and use it over the application:
```
export const ContextNameContext = React.createContext()

export const ContextNameProvider= (children) => {
...(sth. with useState probably)

return <ContextName.Provider value={...}>
{children}
</ContextName.Provider>
}
```

Destructure any feature into a costum component:
```
<a href="..."> text </a> to 
 ...
<LinkText href={...} text={...}/>
...
const LinkText = ({href,text}) => <a href={href]> {text] </a>
```

Absolute imports
- https://medium.com/hackernoon/absolute-imports-with-create-react-app-4c6cfb66c35d


## Python Patterns

- Still to follow.


