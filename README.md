## Haskell Notes
### Application typeclass
<*>: <*> takes a functor that has a function in it and another functor and extracts that function from the first functor and then maps it over the second one.

```haskell
ghci> pure (+) <*> Just 3 <*> Just 5
Just 8
ghci> pure (+) <*> Just 3 <*> Nothing
Nothing
ghci> pure (+) <*> Nothing <*> Just 5
Nothing
```

<$>: fmap as an infix operator
```haskell
ghci> (++) <$> Just "johntra" <*> Just "volta"
Just "johntravolta"
```

`data` :
```haskell
```

`type` :
```haskell
```

`newtype` :
```haskell
```

`class` :
```haskell
class _ a where
  _ :: _ -> _
  
```

`instance` :
```haskell
instance _ _ where
```
