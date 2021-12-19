# go-lessons


启动  
go run main.go  

mysql 数据库文件  
./data/demo.sql  

1.有数据的情况  
curl http://127.0.0.1:8080/getuser/1  
2.报错的情况        
curl http://127.0.0.1:8080/getuser/3

说明 

1. 我们在数据库操作的时候，比如 dao 层中当遇到一个 sql.ErrNoRows 的时候，是否应该 Wrap 这个 error，抛给上层。为什么，应该怎么做请写出代码？