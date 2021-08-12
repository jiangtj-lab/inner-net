# inner-net

自用内部网络代理，基于 spring-cloud-gateway

在 application-net.yml 中添加

```yml
spring:
  cloud:
    gateway:
      routes:
        - id: host_route
          uri: http://localhost:8080
          predicates:
            - Host=example.com
```
