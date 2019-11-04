# Adventures with Julia

I am slowly making my way through the online [v1.2 manual](https://docs.julialang.org/en/v1.2/).

## Gotchas

### 1 / 0 == Inf

The Julia manual
[says](https://docs.julialang.org/en/v1.2/manual/integers-and-floating-point-numbers/#Division-errors-1) that dividing
by zero produces a `DivideError`. However, I observed this:

```julia
julia> 1 / 0
Inf
```

Aaah! Danger! Why?? Well, maybe `Inf` at least is a special weird type that somehow kicks the `DivideError` can down
 the road in some manner? What's it's type? 

```julia
julia> typeof(1 / 0)
Float64
```

Aaah! Why?? I'm not sure what's going on here. Yes, I don't normally divide by zero, but will this behavior be the
 source of subtle bugs? The manual spec makes sense, but trying `1 / 0` in the Julia REPL tells a different story
 . What's going on here?

### typemax(Int64) + 1 == typemin(Int64)

Arithmetic is Julia is a modular arithmetic -- things "wrap around":

```julia
julia> x = typemax(Int64)
9223372036854775807

julia> x + 1
-9223372036854775808

julia> x + 1 == typemin(Int64)
true
```

Comparing with Python:

```python
> from sys import maxsize
> maxsize
9223372036854775807

> maxsize + 1
9223372036854775808
```

Why?? Okay, something to keep in mind.