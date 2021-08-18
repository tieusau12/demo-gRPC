# grpc-java
Demo test gRPC 
RPC ( Remote Procedure Calls)

-gRPC là 1 frameword dành cho RPC của Google.
- là sự kết hợp giữ Protocol Buffers và http2
- giúp giảm tải việc giao tiếp liên tục giữa các service, để các service với nhau tốt độ cao nhất, giảm tải encode/decode data.

- Nên dùng để giao tiếp backend to backend


Protocol buffers là xác định cấu trúc dữ liệu muốn serialize trong 1 file proto. Dữ liệu protocol buffers được cấu trúc như các message, trong đó mỗi message là một bản ghi logic thông tin nhỏ chứa một loạt các cặp name-value được gọi là các fields.

Có nhiều phiên bản: thường dùng thì dùng proto3, hỗ trợ nhiều ngôn ngữ khác nhau,
Đặc điểm của protobuf :
+ Dữ liệu rất dày đặc, đầu ra nhỏ.
+ Khó decode mà không biết schema, định dạng dữ liệu không rõ ràng và cần schema để biết rõ.
+ Xử lý rất nhanh, nhỏ hơn 3 - 10 lần so với XML hoặc JSON
không dành cho con người vì là Binary.
+ Tạo các code truy cập dữ liệu dễ sử dụng hơn theo chương trình.