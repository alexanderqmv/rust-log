# rust-log
Rust-Log: A simple Logging system for Rust!
```rs
#[macro_use]
mod logger;

use logger::{
  LogLevel,
  Logger
};

fn main() {
    // Creating new Logger instance
    let mut logger = Logger::new(LogLevel::Info);
    // Example using macros!

    info!(logger, "This is an info message");
    warn!(logger, "This is a warning message");
    debug!(logger, "This is a debug message");
    error!(logger, "This is an error message");

    // Example гsing a class object to access functions
    logger.warn("This is a warning message [SELF]");
}
```
