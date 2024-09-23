# Snake-Game

I developed this small project for a class in uni. The project is a simple adaptation of the famous snake game. 
The game was builed using:
* an ESP32
* 4 push buttons
* a buzzer
* a SSD1306 screen
  
The following libraries are required for the code to work:
 ` Adafruit_GFX.h `
 ` Adafruit_SSD1306.h `
which you can add directly from Arduino IDE.

This table show the corespondence between the ESP32, the screen, the push buttons and the buzzer:
| ESP32 pin | External Component |
|-----------|-----------|
|GND | GND screen, buttons, buzzer|
| 21 | SDA - screen|
| 22 | SCL - screen|
| 3V3 | VCC - screen|
| 33 | buton - up| 
| 32 | buton - down|
| 26 | buton - left|
| 25 | buton - right|
| 4 | buzzer |

![image](https://github.com/user-attachments/assets/e8421ceb-cea5-4fc2-848f-60ac8ccad09c)

**NOTE** The directions (up, down, left, right) are the possible directions in which the snake can go.

The principle of the game is unchanged: the snake must eat as many fruits as possible without intersecting itself or hitting the walls.
The buzzer have 3 types of sounds: one for the start, on for eating a fruit and one for losing. The score is visibile in the left corner. 

**ATTENTION** Some fruits can apper under the score.

When you lose, you can start a new game by simply pressing the up button once and the game will restart. 






