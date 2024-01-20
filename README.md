# Hello, world!


- 🌱 TypeScript
- 👯 Rust

Experienced on the full-stack, focused on interfaces engineering.

# crust
```rust
fn main() {
    lambda!(handler)
}

fn handler(event: Value, _: Context) -> Result<String, HandlerError> {
    match (event["username"].as_str(), event["password"].as_str()) {
        (Some(username), Some(password)) => {
            match auth::authenticate(username, password) {
                Ok(token) => Ok(token),
                Err(msg) => Err(HandlerError::from(msg)),
            }
        },
        _ => Err(HandlerError::from("Invalid request")),
    }
}
```
