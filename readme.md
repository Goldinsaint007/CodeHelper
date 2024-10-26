# Pin Operations and Optimizations

## Using Int's Declaration Types

- ## Single
``` cpp
// LED Pins - Outputs
int LED_1 = 12;
int LED_2 = 17;
int LED_3 = 13;
int LED_4 = 14;

// BUTTON Pins - Inputs
int Btn_1 = 9;
int Btn_2 = 3;
int Btn_3 = 2;
int Btn_4 = 5;
```

### Use
``` cpp
void setup() {
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);

  pinMode(Btn_1, INPUT);
  pinMode(Btn_2, INPUT);
  pinMode(Btn_3, INPUT);
  pinMode(Btn_4, INPUT);
}
```

### Full Code
``` cpp
#include <Arduino.h>

// LED Pins - Outputs
int LED_1 = 12;
int LED_2 = 17;
int LED_3 = 13;
int LED_4 = 14;

// BUTTON Pins - Inputs
int Btn_1 = 9;
int Btn_2 = 3;
int Btn_3 = 2;
int Btn_4 = 5;

void setup() {
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);

  pinMode(Btn_1, INPUT);
  pinMode(Btn_2, INPUT);
  pinMode(Btn_3, INPUT);
  pinMode(Btn_4, INPUT);
}

void loop() {

}
```

- ## Inline
``` cpp
// LED Pins - Outputs
int LED_1 = 12, LED_2 = 17, LED_3 = 13, LED_4 = 14;

// BUTTON Pins - Inputs
int Btn_1 = 9, Btn_2 = 3, Btn_3 = 2, Btn_4 = 5;
```

### Use
``` cpp
void setup() {
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);

  pinMode(Btn_1, INPUT);
  pinMode(Btn_2, INPUT);
  pinMode(Btn_3, INPUT);
  pinMode(Btn_4, INPUT);
}
```

### Full Code
``` cpp
#include <Arduino.h>

// LED Pins - Outputs
int LED_1 = 12, LED_2 = 17, LED_3 = 13, LED_4 = 14;

// BUTTON Pins - Inputs
int Btn_1 = 9, Btn_2 = 3, Btn_3 = 2, Btn_4 = 5;

void setup() {
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);

  pinMode(Btn_1, INPUT);
  pinMode(Btn_2, INPUT);
  pinMode(Btn_3, INPUT);
  pinMode(Btn_4, INPUT);
}

void loop() {

}
```

- ## Array
``` cpp
// LED Pins - Outputs
int LED[4] = {12, 17, 13, 14};

// BUTTON Pins - Inputs
int Btn[4] = {9, 3, 2, 5};
```

### Use
``` cpp
void setup() {
  for(int i; i < 4; i++) {
    pinMode(LED[[i]], OUTPUT);
  }

  for(int i; i < 4; i++) {
    pinMode(Btn[[i]], OUTPUT);
  }
}
```

### Full Code
``` cpp
#include <Arduino.h>

// LED Pins - Outputs
int LED_1 = 12, LED_2 = 17, LED_3 = 13, LED_4 = 14;

// BUTTON Pins - Inputs
int Btn_1 = 9, Btn_2 = 3, Btn_3 = 2, Btn_4 = 5;

void setup() {
  for(int i; i < 4; i++) {
    pinMode(LED[[i]], OUTPUT);
  }

  for(int i; i < 4; i++) {
    pinMode(Btn[[i]], OUTPUT);
  }
}

void loop() {

}
```