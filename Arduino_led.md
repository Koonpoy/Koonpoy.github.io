## C/C++ Programming Arduino LED

### LED changing pattern: A

- Step 1. Initially, only one LED (at index=0) is ON, and the rest of the LEDs are OFF.
- Step 2. The position of the ON LED should be moved to the next in a circular manner in a fixed time interval and then repeat Step 2.

```
// LED changing pattern: A


const int LED_PINS[] = {5,18,19,21} ;
const int NUM_LEDS = sizeof(LED_PINS)/sizeof(int) ; 

#define OFF (LOW) 
#define ON (HIGH)

void setup() { 
  for (int i=0 ; i < NUM_LEDS ; i++) {
    pinMode(LED_PINS[i], OUTPUT);
    digitalWrite(LED_PINS[i] , (i==0) ? ON:OFF);
  }
}

void loop() {
  for(int i=0 ; i < NUM_LEDS ; i++) {
    digitalWrite(LED_PINS[i], ON);
    delay(1500);
    digitalWrite(LED_PINS[i],OFF);

  }
}
```

#### gif_A

### LED changing pattern: B

Step 1. Initially, all LEDs are OFF.
Step 2. Turn on the LEDs one by one with a time delay, starting at index=0 until all LEDs are ON.
Step 3. If all LEDs are ON, turn off LEDs one by one starting at index=n-1,  where n is the total number of LEDs, until all LEDs are OFF, and repeat Steps 2-3.

```
// LED changing pattern: B

const int LED_PINS[] = {5,18,19,21} ;
const int NUM_LEDS = sizeof(LED_PINS)/sizeof(int) ; 

#define OFF (LOW) 
#define ON (HIGH)


void setup() {
  // put your setup code here, to run once:
    for (int i=0 ; i < NUM_LEDS ; i++) {
    pinMode(LED_PINS[i], OUTPUT);
    }

}


void loop() {
  // put your main code here, to run repeatedly:
  int i = 0;
  for ( i ; i < NUM_LEDS ; i++){
    digitalWrite(LED_PINS[i],ON);
    delay(1000);

  }
  if (i == NUM_LEDS) {
    for ( i-- ; i >= 0; i--){
    digitalWrite(LED_PINS[i],OFF);
    delay(1000);
  }

  }
}
```

#### gif_B

### LED changing pattern: C

Step 1. Initially, all LEDs are OFF.
Step 2. Turn on the first LED by increasing the duty cycle of the PWM signal driving the LED, until the LED is fully ON.
Step 3. Repeat Step 2 with the next LED until all LEDs are fully ON.
Step 4. If all LEDs are ON, turn off LEDs one-by-one by decreasing the duty cycles of the PWM signals until all LEDs are OFF and repeat Steps 2-4.

#### image and gif

### LED changing pattern: D

Step 1. Initially, all LEDs are OFF.
Step 2. Turn on the first 4 LEDs using PWM signals, each with different duty cycles (e.g. 100%, 50%, 25%, 10%), and the rest of the LEDs are OFF.
Step 3. Move the positions of ON LEDs to the left by one position in a circular manner and repeat Step 3.

```
const int LED_PINS[] = {34,35,32,33} ;
const int NUM_PINS = sizeof(LED_PINS)/sizeof(int) ;
const int PWM_RESOLUTION = 8 ;
const int DUTY_MAX = 1 << (PWM_RESOLUTION) ;
const int PWM_FREQ = 5000 ;
const int DUTY_PERCENT[] = { DUTY_MAX /* 100% */ , DUTY_MAX*0.5 /* 50% */ , DUTY_MAX*0.25 /* 25% */, DUTY_MAX*0.1 /* 10% */ } ;
const int NUM_DUTY = sizeof(DUTY_PERCENT)/sizeof(int) ;

void setup() {
  // put your setup code here, to run once:
  for(int i=0 ; i < NUM_PINS ; i++) {
    pinMode(LED_PINS[i] , OUTPUT);
    ledcSetup(i,PWM_FREQ,PWM_RESOLUTION) ;
    ledcAttachPin(LED_PINS[i],i) ;
      for (int x=0 ; x < NUM_DUTY ; x++){
        ledcWrite(i,DUTY_PERCENT[x]);
        delay(100);

  }
  }
  
}

void loop() {
  // put your main code here, to run repeatedly:
}

```

#### gif_D





