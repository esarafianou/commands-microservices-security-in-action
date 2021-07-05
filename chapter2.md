
## 2.1.4 Accessing the Order Processing microservices

```
curl -v http://localhost:8080/orders -H "Content-Type: application/json" --data-binary @- << EOF
{ "items": [{"itemCode": "IT001", "quantity": 3}, {"itemCode": "IT004", "quantity": 1}], "shippingAddress": "No 4, Castro Street, Mountain View, CA, USA"}
EOF
```

## 2.2.3 Getting an access token from the OAuth 2.0 authorization server

```
curl -u orderprocessingapp:orderprocessingappsecret -H "Content-Type: application/json" -d '{"grant_type": "client_credentials", "scope": "read write"}' http://localhost:8085/oauth/token
```

## 2.3.2 Running the sample

Same as 2.1.4
```
curl -v http://localhost:8080/orders -H "Content-Type: application/json" --data-binary @- << EOF
{ "items": [{"itemCode": "IT001", "quantity": 3}, {"itemCode": "IT004", "quantity": 1}], "shippingAddress": "No 4, Castro Street, Mountain View, CA, USA"}
EOF
```
