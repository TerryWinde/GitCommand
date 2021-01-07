# Live Templates

- Header

```java
/**
* Create by Terry on $date$
*/
```

- newInstance
  Creates an instance of the fragment with arguments

```kotlin
companion object {
    fun newInstance($args$): $fragment$ {
      val args = android.os.Bundle()
      $nullChecks$
      $addArgs$
      val fragment = $fragment$()
      fragment.arguments = args
      return fragment
    }
}
```
- singleInstance
```java
private static volatile $NAME$ singleton = null;

private $NAME$() {}

public static $NAME$ getInstance() {
    if (singleton == null) {
        synchronized ($NAME$.class) {
            if (singleton == null) {
                singleton = new $NAME$();
            }
        }
    }
    return singleton;
}
```
