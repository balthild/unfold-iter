# unfold-iter

[![Crates.io](https://img.shields.io/crates/v/unfold-iter.svg)](https://crates.io/crates/unfold-iter)
[![Docs.rs](https://img.shields.io/docsrs/unfold-iter.svg)](https://docs.rs/unfold-iter)
[![License](https://img.shields.io/crates/l/unfold-iter.svg)](LICENSE)

Create iterators with an initial value and a recurrence relation.

## Examples

```rust
use unfold_iter::unfold;

for x in unfold(2, |&x| x * 2).take(5) {
    println!("{}", x);
}

// 2, 4, 8, 16, 32
```
