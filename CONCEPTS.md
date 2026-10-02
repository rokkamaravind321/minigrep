# Rust core concepts checklist

Tick a box when the concept is used in real code, and link the commit.
Stuck on a concept? The matching chapter of [100 Exercises To Learn Rust](https://rust-exercises.com/100-exercises/) is the drill reference.

## Project 1 — minigrep (this repo)
- [ ] Cargo, crates, `main.rs` vs `lib.rs`, modules
- [x] Ownership & moves — step 1
- [x] Borrowing: `&T` vs `&mut T` — step 1 (`&T` only so far)
- [x] `String` vs `&str`, slices — step 2 (concept; used for real in step 4)
- [ ] Structs & `impl` blocks
- [ ] Enums, `Option`, `Result`
- [ ] Pattern matching (`match`, `if let`)
- [ ] Error handling: `?`, `Box<dyn Error>`
- [ ] Lifetimes (basic, in function signatures)
- [ ] Iterators & closures
- [ ] Unit tests & integration tests
- [ ] Using external crates (`clap`)

## Project 2 — generic collections (LRU cache + linked list)
- [ ] Generics & trait bounds
- [ ] Defining & implementing traits
- [ ] Trait objects (`dyn Trait`) vs generics
- [ ] `Box`, `Rc`, `RefCell`, `Weak`
- [ ] Interior mutability
- [ ] Implementing `Iterator`, `Display`, `From`, `Drop`
- [ ] Lifetimes in structs
- [ ] Doc tests
- [ ] Intro to `unsafe`

## Project 3 — multithreaded HTTP server
- [ ] Threads (`std::thread`)
- [ ] `Arc`, `Mutex`, `RwLock`
- [ ] Channels (`mpsc`)
- [ ] `Send` & `Sync`
- [ ] `Fn` / `FnMut` / `FnOnce`, `move` closures
- [ ] Thread pool & graceful shutdown

## Project 4 — Redis clone (tokio)
- [ ] `async`/`await`, `Future`
- [ ] tokio runtime, tasks, TCP
- [ ] Byte parsing (RESP protocol)
- [ ] Custom error types (`thiserror`)
- [ ] Persistence to disk
- [ ] Logging with `tracing`
- [ ] Benchmarks with `criterion`

## Project 5 — advanced
- [ ] Declarative macros (`macro_rules!`)
- [ ] Procedural macros (derive)
- [ ] `unsafe` & FFI
- [ ] `Pin` & writing a tiny executor
