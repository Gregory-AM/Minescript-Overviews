# Doing math in Pyjinn

## No python modules

Pyjinn is compiled into Java, meaning that it has some limitations. One of these is that you cannot use the built-in python modules such as `math`.

To get around this, you can still use Java's built-in math library.

## Initializing

To initialize Java's math module, simply include the following line in your pyjinn file.

```
Math = JavaClass("java.lang.Math")
```

## Documentation

To find available functions, visit:

`https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Math.html`

## Accessing

This `Math` module can be accessed similarly to the python module.

```
x_offset = Math.sin(20) * radius
```

As a reminder, all trig functions use radians as their unit of measurement, not degrees. Convert between them with `Math.toRadians(degrees)`
