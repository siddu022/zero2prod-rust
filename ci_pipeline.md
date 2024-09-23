## *** Continuous Integration empowers each member of the team to integrate their changes into the main branch multiple times a day. ***

- it reduces the chances of having to sort out messy merge conflicts due to long-lived branches.
- ** Continuous Integration (CI) tightens the feedback loop.

### How do we make it possible?
- with a collection of automated checks running on every commit - our CI pipeline. if one of the checks fails you cannot merge to main.

- CI pipelines often go beyond ensuring code health: they are a good place to perform a series of additional important checks 
 e.g. scanning our dependency tree for known vulnerabilities, linting, formatting, etc.



# CI Steps:
1. ** Build: ** compile the code and run the tests. or run the tests only.
```cargo test```

2. Code Coverage: it is a quick way to see how much of your code is covered by tests.
```cargo install cargo-tarpaulin```
```cargo tarpaulin --ignore-tests```

3. ** Linting: ** it is a way to enforce a set of rules on your codebase. 
```rustup component add clippy```
```cargo clippy```
 * if CI pipelines fails due to clippy, you can run ```cargo clippy --fix``` to fix the issues.
 * if CI pipeline would like to fail the linter check if clippy emits any warnings, you can run ```cargo clippy -- -D warnings```

4. ** Formatting: ** it is a way to enforce a consistent style across your codebase.

5. ** Security: ** it is a way to ensure that your dependencies are secure.
```cargo install cargo-audit```
```cargo audit```


