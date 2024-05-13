## Installation

```bash
$ npm install
```

## Generate code from .protofile

disable any flag if needed

change {{name}} with your proto file's name

change directory into protos folder and run this command to generate ts file

```bash
$ cd common/protos
## Window
$ protoc --plugin=protoc-gen-ts_proto=..\..\node_modules\.bin\protoc-gen-ts_proto.cmd --ts_proto_out=../entities --ts_proto_opt=nestJs=true --ts_proto_opt=useDate=true {{name}}.proto
## Mac
$ protoc --plugin=../../node_modules/.bin/protoc-gen-ts_proto --ts_proto_out=../entities --ts_proto_opt=nestJs=true --ts_proto_opt=useDate=true {{name}}.proto
```

## Before publish new version

```bash
$ tsc -b
```

update version in package.json

push this change to remote

## Publish new version

```bash
$ npm publish
```
