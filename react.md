# react syntax

- component syntax
```jsx
function App(){
    return <div> {/* html elements */}
        <Header /> {/* custom elements */}
        hello world!
    </div>
}
```

- useState hook!
```jsx
function App(){
    const [text, setText] = useState('')
    return <div>
        <input value={text} 
            onChange={setText(e.target.value)}
        />
    </div>
}
```

- useEffect hook!
- and "map"
```jsx
function App(){
    const [messages, setMessages] = useState([])

    useEffect(async()=>{
        const msgs = await api.getMessages()
        setMessages(msgs)
    },[]) // empty array here!!! will run ONCE

    return <div>
        {messages.map((m,i)=>{
            // return a component and pass props
            // inside Message, each property of "m"
            // will be available in props.x
            return <Message key={i} {...m} />
        })}
    </div>
}
```