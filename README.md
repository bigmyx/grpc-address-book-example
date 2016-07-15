# grpc-address-book-example

Following the tutorial:
https://developers.google.com/protocol-buffers/docs/gotutorial

Examples files
https://github.com/google/protobuf/tree/master/examples

To generate **addressbook.pb.go** file

The protoc binary file was donwloaded from [github.com/google/protobuf](https://github.com/google/protobuf/releases) releases

```
./protoc --go_out=plugins=grpc:. addressbook.proto
```

This generates addressbook.pb.go in your specified destination directory.

### Run

```
go run add_person.go myBook
```

```
go run list_people.go myBook
```
