## we use actix-web to build a web server

```
#[tokio::main] 
async fn main() -> std::io::Result<()> {
    HttpServer::new(|| {
        App::new()
            .route("/", web::get().to(|| HttpResponse::Ok().body("Hello world")))
    })
    .bind("127.0.0.1:8000)?
    .run()
    .await
} ```
```

```
