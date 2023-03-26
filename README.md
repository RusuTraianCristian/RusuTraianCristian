# Hello, world!


- 🌱 I’m currently learning Rust & GO and aspiring to write a high level framework in Rust
- 👯 I’m looking to collaborate on interesting Rust projects

Currently a part time software engineer @Convect, a software development agency founded by myself.

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
