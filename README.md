<b>WHAT IS THE PROJECT ABOUT?</b><br>
This is a project designed to control an WS2812B LED strip based on sound input, using Fast Fourier Transform (FFT) to analyze the sound frequencies detected by a sound sensor connected to an Arduino. <br>
<b>CODE EXPLANATION</b> <br>
The `arduinoFFT` library is used to perform FFT on sampled sound data to extract frequency components, and the `Adafruit_NeoPixel` library is used to control the LED strip. The sound data is continuously read, and each set of samples is processed using FFT to identify the dominant frequency. The brightness and color of the LED strip are dynamically adjusted based on the sound intensity and frequency. If the sound intensity is below a defined threshold (`sound_thresh`), the LEDs are dimmed; otherwise, the color of the LEDs is determined by mapping the frequency to RGB values, creating a visual effect that reacts to sound. The code loops this process, updating the LED strip in real-time as it receives sound input.<br>
<b>HARDWARE COMPONENTS</b> <br>
1.ARDUINO UNO<br>
2.WS2812B LED STRIP<br>
3.5V EXTERNAL POWER SUPPLY <br>
4.SOUND SENSOR MODULE(preferrably the ky-038 sound sensor module)<br>
<b>HOW TO GET STARTED</b><br>
The components are connected in the following way:<br>
<b>NB!THE POTENTIOMETER IS USED TO REPRESENT THE SOUND SENSOR MODULE</b><br>
![My Image](./schematics/MUSIC%20INTERACTIVE%20LED.PNG) <br>


