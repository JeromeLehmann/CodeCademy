## Java Quiz

#### Q1. What is the result of this zero division?

```java
System.out.println((double)-5 / (double)0);
```

- [ ] Exception in thread "main" java.lang.ArithmeticException: / by zero
- [ ] NEGATIVE_INFINITY
- [ ] NaN
- [ ] MIN_VALUE
- [x] -Infinity

Explanation:
  - 5/0 returns Exception
  + (float)5/0  or 5/(float)0  returns Infinity
  + (double)5/0 or 5/(double)0 returns Infinity

Further reading: https://www.baeldung.com/java-division-by-zero
