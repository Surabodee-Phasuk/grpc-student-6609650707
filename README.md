# grpc-student-6609650707

พัฒนาด้วย **Go** และ **gRPC** เพื่อการเรียนรู้การสื่อสารแบบ Microservices

## 🛠 Assignments Detail
* **Task 1: ListStudents** - เพิ่ม RPC Method สำหรับดึงข้อมูลนักเรียนทั้งหมดในรูปแบบ List (Repeated field)
* **Task 2: New Field (Phone)** - เพิ่มฟิลด์เบอร์โทรศัพท์ (`phone`) เข้าไปในโครงสร้างข้อมูล

## 🏗 Project Architecture

* `proto/`: นิยาม Service และ Message
* `server/`: ส่วนการประมวลผล gRPC Server
* `client/`: ส่วนเรียกใช้งาน gRPC Client

## 🚀 How to Run
1. จัดการ Dependencies: `go mod tidy`
2. Generate Code: `protoc --go_out=. --go-grpc_out=. proto/student.proto`
3. รัน Server: `go run server/server.go`
4. รัน Client: `go run client/client.go`

## 🧪 Testing with Postman
เลือกประเภท Request เป็น gRPC
ระบุ URL เป็น `localhost:50051` และ Import ไฟล์ `proto/student.proto` เพื่อทดสอบฟังก์ชันต่างๆ

---
