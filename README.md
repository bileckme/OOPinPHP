# OOP in PHP

## Basic OOP
Understanding basic object-orientation in PHP

```
abstract class A 
{
  function X()
}
```

```
interface B
{
  function Y()
}
```

```
class C extends A
{
  function Z() 
}
```

```
class D implement B
{
  - have to declare method Y
}
```

```
class E extends D
{
  - have to declare method Y
}
```

```
class F extends A implements B
{
  - has access to method X
  - have to declare method Y
}
```

```
class G extends C
{
  - has access to method X
  - has access to method Z
}
```

```
abstract class H extends A 
{
  - has access to method X (as well)
}
```

```
abstract final class Z
{

}
```

```
class Foo extends Z 
{
  - this cannot be possible because Z is marked as final
}
```

You can extend any class as long as its not marked as `final`.
