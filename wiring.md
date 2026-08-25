# Wiring

| Pins | Of | Pins | Of |
|---|---|---|---|
| IN1 | L298N #1 | - | ESP32-S3 CAM |
| IN2 | L298N #1 | - | ESP32-S3 CAM |
| IN1 | L298N #2 | - | ESP32-S3 CAM |
| IN2 | L298N #2 | - | ESP32-S3 CAM |
| ENA | L298N #1 | - | ESP32-S3 CAM |
| ENA | L298N #2 | - | ESP32-S3 CAM |
| VCC | 1st HC-SR04 | OUT+ | LM2596 |
| VCC | 2nd HC-SR04 | OUT+ | LM2596 |
| VCC | PCA9685 | 3.3V | ESP32-S3 CAM |
| SDA | PCA9685 | - | ESP32-S3 CAM |
| SCL | PCA9685 | - | ESP32-S3 CAM |
| TRIG | 1st HC-SR04 | - | ESP32-S3 CAM |
| TRIG | 2nd HC-SR04 | - | ESP32-S3 CAM |
| ECHO | 1st HC-SR04 | - | ESP32-S3 CAM |
| ECHO | 2nd HC-SR04 | - | ESP32-S3 CAM |
| OUT+ | LM2596 | 5V | ESP32-S3 CAM |
| Positive | battery 1 | B+ | 2S 10A BMS |
| Positive | battery 2 | B+ | 2S 5A BMS |
| Negative | battery 2 | B- | 2S 5A BMS |
| P+ | 2S 10A BMS | 12V | L298N #1 |
| P+ | 2S 10A BMS | 12V | L298N #2 |
| P+ | 2S 5A BMS | IN+ | LM2596 |
| P- | 2S 5A BMS | GND | Common Ground |
| P- | 2S 10A BMS | GND | Common Ground |
| OUT+ | LM2596 | 5V | L298N #1 |
| OUT+ | LM2596 | 5V | L298N #2 |
| Long leg | Capacitor | V+ | PCA9685(External) |
| Short leg | Capacitor | GND | PCA9685(External) |
| GND | L298N #1 | - | Common Ground |
| GND | L298N #2 | - | Common Ground |
| OE | PCA9685 | V+ | PCA9685 (External) |
| Positive | 4 AA battery | V+ | PCA9685 (External) |
| OUT1 | L298N #1 | 1st wire | Left side Motors |
| OUT2 | L298N #1 | 2nd wire | Left side Motors |
| OUT1 | L298N #2 | 1st wire | Right side Motors |
| OUT2 | L298N #2 | 2nd wire | Right side Motors |
| Red wire | Servo | V+ | PCA9685 (Internal) |
| Yellow/Orange wire | Servo | PWM/Signal | PCA9685 (Internal) |
| Brown/Black wire | Servo | GND | PCA9685 (Internal) |
| - | ESP32-S3 CAM | - | Common Ground |
| - | ESP32-S3 CAM | - | Common Ground |
| Negative | battery 1 | B- | 2S 10A BMS |
| Negative | 4 AA battery | - | Common Ground |
| IN- | LM2596 | GND | Common Ground |
| OUT- | LM2596 | GND | Common Ground |
| GND | HC-SR04 | GND | Common Ground |
| GND | ESP32-S3 CAM | GND | Common Ground |
| GND | PCA9685 | GND | Common Ground |

**Note**: In the path of GPIO input pin and ECHO pin of HC-SR04, there must be a resistor of  1kΩ.And the GPIO input pin and Common ground connected through 2kΩ. Select ESP32S3 as a board type, then select ESP32S3 dev module and Give value of property in settings which is given here. The capacitor should be 470µF – 1000µF (electrolytic). The pins BM of BMS board should be connected with middle point of series.

| Servo | Channel |
|---|---|
| Pan servo | CH1 |
| Tilt servo | CH0 |
| Sans servo | CH2 |
