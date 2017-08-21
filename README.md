# buck-config-test

Here is how `.buckconfig` files are merged:

## `.buckconfig`

```
[a]
  x = 1

[b]
  y = 2
  w = 1
```

## `.buckconfig.local`

```
[b]
  y = 7

[c]
  z = 3
```

## Result

```
[a]
  x = 1

[b]
  y = 7

[c]
  z = 3
```
