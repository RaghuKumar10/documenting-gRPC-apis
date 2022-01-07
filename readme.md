Method 1

        creating with protoc-gen-doc docker image
        https://github.com/pseudomuto/protoc-gen-doc

        docker run --rm \
            -v $(pwd)/documenting-gRPC-apis/doc:/out \
            -v $(pwd)/documenting-gRPC-apis/proto:/protos \
            pseudomuto/protoc-gen-doc

        sudo docker run --rm \
            -v $(pwd)/documenting-gRPC-apis/doc:/out \
            -v $(pwd)/documenting-gRPC-apis/proto:/protos \
            pseudomuto/protoc-gen-doc --doc_opt=json,description.json

Method 2

        https://blog.gendocu.com/posts/documenting-grpc/
