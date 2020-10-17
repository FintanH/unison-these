# unison-these

A `These` representation in Unison, inspired by the Haskell [`these`](https://hackage.haskell.org/package/these) package.

# What are These?

`These` consists of a simple sum-type with three variants. The first two variants are reminiscent of `Either`,
while the third variant is allowed to hold both the `a` and `b`. Here it is defined in Unison:

```
type These a b = This a | That b | These a b
```

## Example Use Case

I wrote about a use case of migration paths once, if you'd like to check it out: [These Changes](https://fintanh.github.io/posts/these-changes.html).
