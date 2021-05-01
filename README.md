# Uname-rs

No dependency, panic-less implementation of the POSIX utsname header and struct in Rust.

Taken from my project [rfetch](https://github.com/caverym/rfetch)

```rust
use std::io::Result;
use uname_rs::Uname;

fn main() -> Result<()> {
	let uts = Uname::new()?;

	println!("{}", uts.sysname);

	Ok(())
}
```
	