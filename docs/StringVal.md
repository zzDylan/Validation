# StringVal

- `v::stringVal()`

Validates whether the input can be used as a string.

```php
v::stringVal()->validate('6'); // true
v::stringVal()->validate('String'); // true
v::stringVal()->validate(1.0); // true
v::stringVal()->validate(42); // true
v::stringVal()->validate(false); // true
v::stringVal()->validate(true); // true
v::stringVal()->validate(new ClassWithToString()); // true if ClassWithToString implements `__toString`
```

***
See also:

  * [Alnum](Alnum.md)
  * [BoolType](BoolType.md)
  * [CallableType](CallableType.md)
  * [FloatType](FloatType.md)
  * [IntType](IntType.md)
  * [NullType](NullType.md)
  * [ObjectType](ObjectType.md)
  * [ResourceType](ResourceType.md)
  * [StringType](Alnum.md)
  * [Type](Type.md)
