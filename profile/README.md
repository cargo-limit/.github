cargo-limit is a cargo plugin that improves Cargo and Rust compiler ergonomics:
- errors have highest priority
    - they never appear in the middle of warnings
    - **warnings are skipped** by default until errors are fixed
    - external [path dependencies'](https://doc.rust-lang.org/cargo/reference/specifying-dependencies.html#specifying-path-dependencies) warnings are skipped by default
- all messages come **in reversed order** by default
    - to avoid extra scrolling
- messages are grouped by filenames
- number of messages can be limited
- after encountering **first error** the rest of **build time is limited** by default
- files can be **[automatically opened](#text-editoride-integrations) in your text editor on affected lines**

Initially this project was a workaround for **[this issue](https://github.com/rust-lang/rust/issues/27189), which was closed with no adequate solution**.

Check out [roadmap](https://github.com/cargo-limit/cargo-limit/projects/1?fullscreen=true), [issues](https://github.com/cargo-limit/cargo-limit/issues) and [🎙️ Rustacean Station podcast episode](https://rustacean-station.org/episode/alexander-lopatin/) for more.
