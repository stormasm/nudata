
The character generated from nushell grid is not the
same character github expects to see for tables...

That is why this does not work...

```rust
help commands | select name | first 25 | grid | to md | save toc.md
```
