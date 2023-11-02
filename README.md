# JSON.tryParse

## Problem to solve

```js
try { return JSON.parse(str) } catch { return undefined }
```

## Prior art

[URL.canParse](https://developer.mozilla.org/en-US/docs/Web/API/URL/canParse_static)

## Spec

```markdown
JSON.parse ( _text_ [ , _reviver_ ] )

1. Let _result_ be Completion(Call(%JSON.parse%, *null*, << _text_, _reviver_ >> )).
1. If _result_ is an abrupt completion, return *undefined*.
1. Return _result_.
```
