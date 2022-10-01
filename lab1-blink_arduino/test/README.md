# Lab 1: Ondřej Nesvadba

### Morse code

1. Listing of C code which repeats one "dot" and one "comma" (BTW, in Morse code it is letter `A`) on a LED. Always use syntax highlighting, meaningful comments, and follow C guidelines:

```c
int main(void)
{
    uint8_t led_value = LOW;  // Local variable to keep LED status

    // Set pin where on-board LED is connected as output
    pinMode(LED_GREEN, OUTPUT);

    uint8_t n = 0;

    // Infinite loop
    while (1)
    {
        // Turn ON/OFF on-board LED
        digitalWrite(LED_GREEN, led_value);
  
        // Pause several milliseconds
        _delay_ms(SHORT_DELAY);

        // Change LED value
        if (led_value == LOW)
            led_value = HIGH;
        else
            n += 1
              if (n==2)
                _delay_ms(2*SHORT_DELAY);
                uint8_t n = 0;
                uint8_t led_value = LOW;

            uint8_t led_value = LOW;
    }

    // Will never reach this
    return 0;
}
```

2. Scheme of Morse code application, i.e. connection of AVR device, LED, resistor, and supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values!

 ![image](https://user-images.githubusercontent.com/99417291/192530439-84f325ec-6886-4576-bcb5-0ca27041c0de.png)
