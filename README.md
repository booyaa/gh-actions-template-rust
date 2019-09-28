# gh-actions-template-rust

A starter template for Rust projects with GitHub Actions CI orientated workflow.

## Usage

- click on the `Use this template` button for this repo
- fill out the new project details
- git clone your new GitHub project
- cd to the project's directory
- initialise with a new Rust project `cargo init --vcs none` alternative copy your existing code into the folder
- update this `README.md` to reflect your own project's awesomeness!

## Why

Continuous Integration (CI) is a way to mitigate potential problems arising from changes to code, dependencies or even version changes to the programming language that powers your awesome project. 

By continuously building and testing your code as changes arrive, you can have confidence that the code you merge won't break your project.`</soapbox>`

Setting up continuous integration pipeline for your projects can be tricky, but using GitHub Actions can make this incredibly easy and not require 3rd party services like [Travis CI][link_travis] or [Circle CI][link_circleci].

If you're wondering why you have to initialise your project using `cargo init` on first use, it's because [Cargo][link_cargo] already does a great job of creating new Rust projects. By not including  the Rust scaffolding, we avoid missing out on changes as they happen to the Cargo new project process.

## What's in the box

- A CI workflow that runs the following cargo commands: `check`, `test`, `fmt` (formatting) and `clippy` (linter) using the latest stable toolchain. All of these actions are configurable, and documentation can be found [here][actionrs_docs]/
- Dual MIT and Apache v2 license, which is how Rust is currently licensed.

## What's not in the box

- A Continuous Delivery (CD) pipeline to tag, create releases and deploy to crates.io (Rust's package repository), this may happen later.
- A Code coverage step, this may happen later.

## Thanks

The GitHub Actions workflow was copied from [actions-rs][link_actionrs]'s excellent [quick start guide][actionrs_quickstart] for GitHub Actions for Rust 

## License

As with Rust, this template is primarily distributed under the terms of both the MIT license
and the Apache License (Version 2.0), with portions covered by various
BSD-like licenses.

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT) for details.

## Copyright

Mark Sta Ana &copy; 2019 

<!-- linkies -->

[link_travis]: https://travis-ci.org
[link_circleci]: https://circleci.com
[link_cargo]: https://doc.rust-lang.org/cargo/index.html
[link_actionrs]: https://github.com/actions-rs
[actionrs_quickstart]: https://github.com/actions-rs/meta/blob/master/recipes/quickstart.md
[actionrs_docs]: https://github.com/actions-rs/meta/blob/master/recipes/quickstart.md#can-i-tune-it
