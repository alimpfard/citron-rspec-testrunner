# Citron Test runner

A minimal old-style RSpec-like test runner

# Merged into [the standard library](https://github.com/alimpfard/citron/tree/master/Library/Test)

```
describe Some stuff do: {:it
    it can maybe fail do: {
        Boolean flip should = True.
    }.

    it can maybe catch errors do: {
        Dice roll > 3 ifTrue: {
            { thisBlock error: ArgumentError['Invalid argument']. }
                should raiseError: ArgumentError.
        }.
    }.
}.
```

All of this is just one `import Test: 'describe'` away!
