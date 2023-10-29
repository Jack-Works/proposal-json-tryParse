# JSON.canParse

## Problem to solve

```js
try { JSON.parse(str) } catch { return false }
return true
```

## Prior art

[URL.canParse](https://developer.mozilla.org/en-US/docs/Web/API/URL/canParse_static)

## Spec

```markdown
1. Let _jsonString_ be ? ToString(*value*).
1. Parse StringToCodePoints(_jsonString_) as a JSON text as specified in ECMA-404.
1. If it is not a valid JSON text as defined in that specification, return *false*.
1. Return *true*.
```
