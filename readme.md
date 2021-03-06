## Installation

Requires [Node.js](https://nodejs.org/)

Install the dependencies and devDependencies and start the server.

For service heroes:

```sh
cd heroes
npm init -y
npm install express body-parser
```

For service threats:

```sh
cd threats
npm init -y
npm install express body-parser
```

## Start projects

For service heroes...:

```sh
node ./heroes/heroes.js 8081
```

For service threats:

```sh
node ./threats/threats.js 8082
```

## Testing service

For service heroes:

```sh
curl -i --request GET localhost:8081/heroes
```

For service threats:

```sh
curl -i --request POST --header "Content-Type: application/json" --data '{"heroId": 1, "threatId": 1}' localhost:8082/assignment
```

## References

[MACIEJ TREDER](https://www.twilio.com/blog/building-javascript-microservices-node-js)
