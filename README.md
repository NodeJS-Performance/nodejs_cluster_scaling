# NodeJS cluster scaling

https://www.digitalocean.com/community/tutorials/how-to-scale-node-js-applications-with-clustering

## To measure the performance of the index.js and primary.js file.:

Open 2 terminals.

In your 1st terminal, run the index.js or primary.js file. It will start the server:

```sh
node index.js
```
or
```sh
node primary.js
```

Next, go to your 2nd terminal to use the loadtest package to send requests to the server:

```sh
loadtest -n 1200 -c 200 -k http://localhost:3000/heavy
```
