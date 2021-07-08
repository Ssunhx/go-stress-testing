#### 增加 method 参数

    如果你不想在 txt 文件中写 curl，可以直接使用 method 参数传入你想要执行的方法
    
    执行 DELETE 
        
        go run main.go -c 10 -n 100 -u 'http://127.0.0.1:3600/xxx/xx?x=111' -method DELETE
    
    执行 POST（没有参数）
        ./go-stress-testing-mac -c 10 -n 100 -u http://127.0.0.1:3600/xxx/xx -method POST
    
    执行 POST （带参数）
        ./go-stress-testing-mac -c 10 -n 100 -u http://127.0.0.1:3600/xxx/xx -method POST -data '{
            "x1": "xxx",
            "x2": "xxx"
        }'