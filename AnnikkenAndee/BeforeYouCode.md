# Before You Code

Congratulations on getting your first Annikken Andee shield! Before you start coding your first project with Annikken Andee, let us introduce to you how to use the library and various steps required for Annikken Andee to work.

**Note:** These steps are required for each project that you use with Annikken Andee. Leaving out these steps results in compile errors.

## Including Libraries

### Andee U/iOS/Android
For every project using Annikken Andee U/iOS/Android, we require the following libraries:

1. SPI.h
2. Andee.h

To include them in the project. Insert the following code snippet at the top of your Arduino sketch.

```cpp
#include <SPI.h>
#include <Andee.h>
```
### Andee 101
For every project using Arduino 101, we require the following libraries:

1. CurieBLE.h
2. Andee101.h

To include them in the project. Insert the following code snippet at the top of your Arduino sketch

```cpp
#include <CurieBLE.h>
#include <Andee101.h>
```

## Starting Andee Communication

Andee communication is required to be started by code. Include the following code into your project. This code only needs to be called once. Therefore, we will add it to the setup() function of Arduino.

For Andee U/iOS/Android
```cpp
void setup() {
    Andee.begin();  // Setup communication between Annikken Andee and Arduino
}
```

For Andee 101
```cpp
void setup() {
    Andee101.begin();  // Setup communication between Annikken Andee and Arduino
}
```

