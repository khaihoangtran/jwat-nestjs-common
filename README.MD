## Installation

```bash
$ npm install
```

## Generate code from .protofile

disable any flag if needed

change {{name}} with your proto file's name

```bash
$ protoc --plugin=protoc-gen-ts_proto=.\node_modules\.bin\protoc-gen-ts_proto.cmd --ts_proto_out=./packages/entities --ts_proto_opt=nestJs=true --ts_proto_opt=useDate=true ./packages/protos/{{name}}.proto
```
