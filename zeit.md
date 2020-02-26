### zeit

- `now --prod` (automatically will detect that you are using create-react-app, and will build it on their server... you dont have to run "npm run build")

### api

- anything in the "api" folder will get deployed as a "zeit serverless function" in the cloud. You can use any programming language. 
- "api/index.js" -> `fetch('/api')`
- "api/weather.js" -> `fetch('/api/weather')`

- the syntax for javascript serverless functions:

```js
module.exports = async function(req,res){
    try {
        // do something
        // req.body = body of the request (for POST)
        // req.query = query parameters (?lat=1.2&lng=2)
        res.status(200).send(response)
    } catch(e) {
        res.status(500).send(e.message)
    }
}
```