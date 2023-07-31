# hyperledger-sawtooth-demo

Run using npm start.

To create a wallet. 
```
curl --location --request POST 'http://localhost:3434/create' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "abc",
    "amount": 199
}'
```
To check the balance
```
curl --location --request POST 'http://localhost:3434/check' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name":"abc"
}'
```

To send a transaction. 
```
curl --location --request POST 'http://localhost:3434/send' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name":"abc",
    "amount":5,
    "receiver": "xyz"
}'
```
