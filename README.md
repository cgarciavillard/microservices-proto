## MicroServices Proto

### Using the Protocol Buffer Compiler

```
  protoc --go_out=./golang --go_opt=paths=source_relative --go-grpc_out=./golang --go-grpc_opt=paths=source_relative ./order/order.proto ./payment/payment.proto ./shipping/shipping.proto
  ```

### Creating GitHub Tags
```
git tag -a tag_name -m "tag description"

git tag -a golang/order/v1.5.0 -m "golang/order/v1.5.0"
git tag -a golang/payment/v1.6.0 -m "golang/payment/v1.6.0"
git tag -a golang/shipping/v1.7.0 -m "golang/shipping/v1.7.0"

git push --tags
```

### Listing GitHub Tags
```
git tag -l
```

### Removing GitHub Tags (Local)
```
git tag -d golang/order/v1.0.0
git tag -d golang/payment/v1.0.0
git tag -d golang/shipping/v1.0.0
```

### Removing GitHub Tags (Remote)
```
git push origin --delete golang/order/v1.0.0
git push origin --delete golang/payment/v1.0.0
git push origin --delete golang/shipping/v1.0.0
```