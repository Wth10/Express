const axios = require('axios')
const cors = require('cors')
const express = require('express')
const app = express()
const port = 5252

app.use(cors())

app.get('/', async(_req, res) => {
  try {
    const {data} = await axios("https://jsonplaceholder.typicode.com/users")
    return res.json(data)
    
  } catch (error) {
    console.error(error)
  }
}
)

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})