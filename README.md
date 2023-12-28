# Using gRPC web in angular

# Compiling `proto` files using `protoc-gen-ts`

Run the following to add messages
```
protoc --plugin=protoc-gen-ts=".\node_modules\.bin\protoc-gen-ts.cmd" --ts_out="import_style=commonjs,binary:generated" --proto_path="protos" my_proto.proto
```

Run the following to add services
```
protoc --plugin=protoc-gen-ts=".\node_modules\.bin\protoc-gen-ts.cmd" --ts_out="service=grpc-web:generated" --proto_path="protos" my_proto.proto
```
