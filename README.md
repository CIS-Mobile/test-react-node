<h1 id="availablescripts">STEP 1 - Getting started</h1>

<h2 id="prerequisites"><code>OPTION 1 - Prerequisites to run REPOs via Docker ( Recommended! )</code></h3>

<p>You will need to install or have the following assets installed on your OS:</p>

<h3 id="prerequisite-docker"> install <a href="https://www.docker.com/products/docker-desktop/">Docker</a> in your OS << Link to download</h3>

<h3 id="initial-repo-setup"><code>Initial Repo Setup</code></h3>
<p>Please run the following two CLI commands to initialize the submodule REPOs</p>
1. <code>git submodule init</code><br/>
2. <code>git submodule update</code><br/>

<h3 id="initial-repo-setup-Docker"><code>Initial Docker Setup</code></h3>
<p>Please run the following two CLI commands to initialize the Docker Environment</p>
<p>Hint: Add 'sudo' at the start if errors received</p>
1. <code>docker-compose build</code><br/>
2. <code>docker-compose up</code><br/>
4. Try to access the frontend via <a href="localhost:3001/">localhost:3001/</a><br/>
5. Use postman to test the login endpoint on the server using the following information:<br/>
<br/>
<code>

    const axios = require('axios');
    let data = JSON.stringify({
        "email": "test@gmail.com",
        "password": "Aa123456!"
    });

    let config = {
        method: 'post',
        maxBodyLength: Infinity,
        url: 'localhost:4000/v1/auth/login',
        headers: {
            'Content-Type': 'application/json'
        },
        data : data
    };

    axios.request(config)
        .then((response) => {
            console.log(JSON.stringify(response.data));
        })
        .catch((error) => {
            console.log(error);
        });

</code>

<h3 id="npmstart">Before you proceed, <u>first confirm that you can login to the frontend</u>, you can ask for help.</h3>

<h2>Whenever you're ready, inform us so we could start the clock.</h2>

<br/><br/><br/><br/>

<h2 id="prerequisites"><code>OPTION 2 - Prerequisites to run REPOs locally</code></h3>

<p>You will need to install or have the following assets installed on your OS:</p>

<h3 id="prerequisite-nodejs"><a href="https://nodejs.org/en/download">Nodejs</a>(tested with V16) << Link to download</h3>
<p>Hint: If you're version is different, consider NVM to change your version easily</p>
<h3 id="prerequisite-mongodb"><a href="https://www.mongodb.com/docs/manual/administration/install-community/">MongoDB</a>(Latest version)  << Link to download</h3>
<p>Note, you will need to know the mongodb URL and credentials, you set these up during install. </p>

<h3 id="initial-repo-setup"><code>Initial Repo Setup</code></h3>
<p>Please run the following two CLI commands to initialize the submodule REPOs</p>
1. <code>git submodule init</code><br/>
2. <code>git submodule update</code><br/>
3. Follow the instructions in each submodule to start both node.js and React. ( cd into them, execute relevant instructions ) </br>
4. Try to access the frontend via <a href="localhost:3001/">localhost:3001/</a>
5. Use postman to test the login endpoint on the server using the following information:<br/>
<br/>
<code>

    const axios = require('axios');
    let data = JSON.stringify({
        "email": "test@gmail.com",
        "password": "Aa123456!"
    });

    let config = {
        method: 'post',
        maxBodyLength: Infinity,
        url: 'localhost:4000/v1/auth/login',
        headers: {
            'Content-Type': 'application/json'
        },
        data : data
    };

    axios.request(config)
        .then((response) => {
            console.log(JSON.stringify(response.data));
        })
        .catch((error) => {
            console.log(error);
        });

</code>

<h3 id="npmstart">Before you proceed, <u>first confirm that you can login to the frontend</u>, you can ask for help.</h3>

<h2>Whenever you're ready, inform us so we could start the clock.</h2>
