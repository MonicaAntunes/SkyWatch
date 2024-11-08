## Studies EXPRESS and AXIOS

<div>
Express - framework for Node.js, used to build server-side applications and API's

Routing: Express allows you to define routes to handle different HTTP mehots(get, post...) and endpoints.
Middleware: Express supports middlwares functions that can process requests and responses at various points in the request-response cycle.
Template Engines: Express can render dynamic HTML pages using template engines like Pug, EJS, etc.
Static FIles: Express cans erve static files such as images, CSS, and JavaScript files.
API Development: Express is commonly used to build REASTful API's.

Installation
npm install express

Example:
Defining route and port.

const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
    res.send('Hello, World!');
});

app.listen(port, () => {
    console.log(`Server is running on http://localhost:${port}`);
});

</div>

<div>
Axios - is a promise-baed HTTP client for the browser and Node.js. It's used to make HTTP requests to external API's or servers.

HTTP Requests: Axios can handle GET, POST PUT, DELETE, and other HTTP methods.
Promise-based: Axios operations return promises, making it easier to handle asynchronous requests.
Interceptors: Axios supports request and response interceptors for preprocessing or logging.
Error Handling: Axios provides built-in mechanisms for handling HTTP errors.
Configuration: Axios allows for global and per-request configuration of headers, timeouts, and other settings.

Installation
npm install axios

Example:

const axios = require('axios');
async function fetchData() {
    try {
        const response = await axios.get('https://jsonplaceholder.typicode.com/posts');
        console.log(response.data);
    } catch (error) {
        console.error('Error fetching data:', error);
    }
}

fetchData();

</div>

<div>
Consulted docs:
https://github.com/axios/axios#axios-api
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction
</div>