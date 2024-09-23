<b>(1)WHAT IS THE PROJECT ABOUT?</b><br>
This is a project designed to control an WS2812B LED strip based on sound input, using Fast Fourier Transform (FFT) to analyze the sound frequencies detected by a sound sensor connected to an Arduino. <br>

<b>(2)CODE EXPLANATION</b> <br>
The `arduinoFFT` library is used to perform FFT on sampled sound data to extract frequency components, and the `Adafruit_NeoPixel` library is used to control the LED strip. The sound data is continuously read, and each set of samples is processed using FFT to identify the dominant frequency. The brightness and color of the LED strip are dynamically adjusted based on the sound intensity and frequency. If the sound intensity is below a defined threshold (`sound_thresh`), the LEDs are dimmed; otherwise, the color of the LEDs is determined by mapping the frequency to RGB values, creating a visual effect that reacts to sound. The code loops this process, updating the LED strip in real-time as it receives sound input.<br>

<b>(3)HARDWARE COMPONENTS</b> <br>
1.ARDUINO UNO<br>
2.WS2812B LED STRIP<br>
3.5V EXTERNAL POWER SUPPLY <br>
4.SOUND SENSOR MODULE(preferrably the ky-038 sound sensor module)<br>

<b>(4)HOW TO GET STARTED- Hardware Components</b><br>

The components are connected in the following way:<br>
<b>NB!THE POTENTIOMETER IS USED TO REPRESENT THE SOUND SENSOR MODULE</b><br>

![My Image](./schematics/MUSIC%20INTERACTIVE%20LED.PNG) <br>
You can find a more detailed pdf schematic in the schematics folder<br>

<b>Explanation</b><br>
(1)The negative wire (ground) of the LED strip is wired to the negative terminal of the external power supply.<br>
(2)The positive wire of the LED strip is wired to the positive terminal of the external power supply.<br>
(3)The data input of the LED strip is wired to Digital pin 6 on the Arduino, enabling communication between the Arduino and the LED strip.<br>
(4)The analog pin (A0) of the sound sensor module is wired to Analog pin A5 on the Arduino.<br>
(5)The ground pin of the sound sensor module is wired to the GND pin on the Arduino.<br>
(6)The positive pin of the sound sensor module is wired to the 3.3V Power pin on the Arduino.<br>

<b>(4)HOW TO GET STARTED- Code</b><br>
-Import the two zip files in the libraries folder onto your Arduino IDE <br>
-Copy the interactive_led.ino code file into the IDE, compile and upload the code into the arduino<br>

