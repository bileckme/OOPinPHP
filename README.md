# OOP in PHP

## Basic OOP
Understanding basic object-orientation in PHP

```
abstract class A 
{
  `methodX`
}
```

```
interface B
{
  `methodY`
}
```

```
class C extends A
{
  `methodZ`
}
```

```
class D implement B
{
  `have to declare methodY`
}
```

```
class E extends D
{
  `have to declare methodY`
}
```

```
class F extends A implements B
{
  `has access to methodX`
  `have to declare methodY`
}
```

```
class G extends C
{
  `has access to methodX`
  `has access to methodZ`
}
```

```
abstract class H extends A 
{
  `has access to methodX (as well)`
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
  `this cannot be possible because Z is marked as final`
}
```

You can extend any class as long as its not marked as `final`.
