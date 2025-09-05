
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest

protoc --go_out=./pkg -I . google/protobuf/field_options.proto
protoc --go_out=./pkg -I . google/protobuf/method_options.proto
protoc --go_out=./pkg -I . google/protobuf/service_options.proto
protoc --go_out=./pkg -I . google/protobuf/queue_response.proto