## Chapter 1

Haskell is a functional programming language. IF you're coming from a C/C++/Java/Python background, things might look a little different in Haskell.

The key thing to note about functional programming is the fact that data/variables in a program remain the same.

Let's say you have a variable `foo`, and that you would like to perform some operation on it, instead of directly changing it, you make a function that returns the modified value. This design pattern looks like it constrains the programmer but in reality, the existence of these constriants makes some problems trivial to solve in haskell which would otherwise need several other steps.

Another benefit is that since capabilites are restricted to isolated functions which may be chained to perform other operations, in case of an error arising in the program, the programmmer can isolate the problem and find the cause for the bug in the program easily.

a function is a first-class citizen in haskell and can be defined as such:

```haskell
f x = x + 3
```

Type enforcement is also possible in haskell and can be done like so:

```
f :: Int -> Int
f :: Float -> Float
-- or more generally,
f :: (Num a) => a -> a
f x = x + x
```
