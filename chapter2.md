
## 2.1.4 Accessing the Order Processing microservices

```
curl -v http://localhost:8080/orders -H "Content-Type: application/json" --data-binary @- << EOF
{ "items": [{"itemCode": "IT001", "quantity": 3}, {"itemCode": "IT004", "quantity": 1}], "shippingAddress": "No 4, Castro Street, Mountain View, CA, USA"}
EOF
```
