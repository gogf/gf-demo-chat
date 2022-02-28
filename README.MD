# A simple MVC chat service

## Installation

### 1. You need a go development environment setup before everything starts taking off.

### 2. Use `git clone` to clone the repo to your local folder. 
```
git clone https://github.com/gogf/gf-demo-chat
```

### 3. Run command `go run main.go`, and you'll see something as follows if success:
```
  ADDRESS | METHOD |      ROUTE      |                                HANDLER                                 |    MIDDLEWARE      
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | ALL    | /*              | github.com/gogf/gf/v2/net/ghttp.internalMiddlewareServerTracing        | GLOBAL MIDDLEWARE  
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | ALL    | /*              | github.com/gogf/gf/v2/net/ghttp.MiddlewareHandlerResponse              | GLOBAL MIDDLEWARE  
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | ALL    | /api.json       | github.com/gogf/gf/v2/net/ghttp.(*Server).openapiSpec                  |                    
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | GET    | /chat           | github.com/gogf/gf-demo-chat/v2/internal/controller.(*hChat).Index     |                    
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | POST   | /chat/name      | github.com/gogf/gf-demo-chat/v2/internal/controller.(*hChat).Name      |                    
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | GET    | /chat/websocket | github.com/gogf/gf-demo-chat/v2/internal/controller.(*hChat).Websocket |                    
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
  :8199   | ALL    | /swagger/*      | github.com/gogf/gf/v2/net/ghttp.(*Server).swaggerUI                    | HOOK_BEFORE_SERVE  
----------|--------|-----------------|------------------------------------------------------------------------|--------------------
```

# GoFrame Sites
### GoFrame Repo
* [https://github.com/gogf/gf](https://github.com/gogf/gf)

### GoFrame Home
* [https://goframe.org](https://goframe.org) (中文)
