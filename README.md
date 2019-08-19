### immutables
---
https://github.com/immutables/immutables/

https://immutables.github.io/

```java
@Value.Immutable
public interface ValueObject extend WithValueObject {
  String getName();
  List<Integer> getCounts();
  Optional<String> getDescription();
  
  class Builder extends ImmutableValueObject.Builder {}
  
}

ValueObject v =
  new ValueObject.Buider()
    .name("Nameless")
    .description("present")
    .addCounts(1)
    .addCounts(2)
    .build();

v = v.withName("Doe");
```

```
```

```
```
