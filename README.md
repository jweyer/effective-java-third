# Effective-Java-Third-Edition-Reading-Notes
Cloned from: https://github.com/AaronLiuIsCool/Effective-Java-Third-Edition-Reading-Notes

* [2-4] Use java.lang.AssertionError ...  Thrown explicitly hen something impossible happens.
    E.g. When a private constructor is called that shouldn't be.
* [] Use java.util.Objects.requireNonNull() to validate constructor and method parameters.
    Checks that the specified object reference is not null and throws a NullPointerException if it is.
* [2-5] Dependency injection is equally applicable to constructors, static factories (Item 1), and builders (Item 2).
* [2-5] Dependency injection framework, such as Dagger [Dagger], Guice [Guice], or Spring [Spring].
* [2-6] Prefer primitives to boxed primitives, and watch out for unintentional autoboxing.
* [2-7] Memory leaks in garbage-collected languages (unintentional object retentions) are insidious.
* [2-8] Finalizers have been deprecated in Java 9.  Cleaners are introduced in Java 9 to replace finalizers.
    ```java
    java.lang.ref.Cleaner
    // Manages a set of object references and corresponding cleaning actions.  
    // Cleaning actions are registered to run after the cleaner is notified that the object has become phantom reachable. 
    ```
* [2-8] Use java.lang.AutoCloseable interface ...
    Closes this resource, relinquishing any underlying resources. This method is invoked automatically on objects managed by the try-with-resources statement.  
    ```java
    void close()
        throws Exception
    ```
* []  