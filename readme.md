# golang

#### so easy to build a website


#### to create a file name index.go
#### index.go
```go
package main

import "net/http"

func main()  {
	http.HandleFunc("/",someFunc)
	http.ListenAndServe(":8080",nil)
}

func someFunc(w http.ResponseWriter, req * http.Request)  {
	w.Write([]byte("Hello universe"))
}
```

```
go run index.go
```