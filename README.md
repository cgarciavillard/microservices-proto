## MicroServices Proto

### Using the Protocol Buffer Compiler

 ```
  protoc \
    --go_out=./golang \
    --go_opt=paths=source_relative \
    --go-grpc_out=./golang \
    --go-grpc_opt=paths=source_relative \
    ./order/order.proto \
    ./payment/payment.proto \
    ./shipping/shipping.proto
  ```

### Creating GitHub Tags
```
git tag -a golang/order/v1.2.3 -m "golang/order/v1.2.3"
git push --tags
```