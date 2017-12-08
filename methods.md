# Defining Methods
Methods allow you to smoothly display code examples in different languages.

{% method %}
## Andee methods
The `Andee` Class has general functions that affects the way the Andee board works or what it does.
{% endmethod %}

{% method %}
### Begin

This function is required to be used before calling any `Andee` functions

```cpp
Andee.begin();
```
This function will setup the SPI communication on the Arduino board. The Slave Select pin will default to pin 8. If the `Andee` Slave Select pin conflicts with another shield, you can use the function below to change it
```cpp
Andee.begin(pin);
```
where `pin` is the Arduino pin to be used as the `Andee` Slave Select pin.
{% endmethod %}

{% method %}
### Change the Bluetooth name on the Andee

This function will change the name of the Andee board. Only works on firmware 2.00 and above
```cpp
Andee.setName(name);
```
where `name` is a character array.
{% endmethod %}

{% method %}
### Clear All Widgets on App

{% endmethod %}












{% method %}
###

{% endmethod %}





{% method %}



{% endmethod %}







My first method exposes how to print a message in JavaScript and Go.

{% sample lang="js" %}
Here is how to print a message to `stdout` using JavaScript.

```js
console.log('My first method');
```

{% sample lang="go" %}
Here is how to print a message to `stdout` using Go.

```go
fmt.Println("My first method")
```

{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
