# Object Detection with Raspberry Pi and Simon Says
What Instant detection of an object, with a confidence level when placed in front of a camera, is what this model does. Using Raspberry Pi, Open CV, and Tensorflow Lite, I was able to run and test an object detection model.

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Hari V | Mission San Jose High School | Computer Science | Incoming Senior

<!---
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**



![Headstone Image](logo.svg)
-->
  
# Final Milestone
My Final milestone includes finalizing the model and using Cad to create a case and a stand for the camera. After the initial testing of the model, I continued testing the model with other, less common objects, to see the range of objects which the model detects, and realized the model only detects more common objects such as electronics, common vehicles, and household items. 
After I finished testing the model and being satisfied with the model, I decided to make a case and a stand for the camera because I had to manually set the camera, and hold it on the table when I was testing it, causing inconvenience. I used the shape to make the case and created a hole around the center of the front face of the case so the camera would be visible and not be blocked by the case. I created a hole on the top of the case so the camera could slide into the case, and I created a hole on the bottom right on the back side of the case so I could plug the camera into the raspberry pi using a connector and a USB cable. I created a stand that was thick enough to hold the case, and sturdy enough so the stand wouldn't break. I created 2 stands, one for each side of the case so it would be sturdy and not too flimsy.
I faced a challenge after the case and stands were printed as I realized the camera was not fitting into the slot in the case as the camera was too thick. I didn't account for the maximum thickness at any 2 points and only accounted for the maximum thickness at a single point causing the camera not to fit fully into the case. This caused me to find a solution, to Dremel. the hole for the connector, all the way to the top of the case, so the connector would slide in and would not be dependent on the thickness of the case. 
For my next modification I would be training my own model and labeling my own pictures using bounding boxes, for a model which differentiates between different types of cars such as an SUV and a pickup truck.
<iframe width="560" height="315" src="https://www.youtube.com/embed/bRFJf-OkRVo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<!--- For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
-->


# Second Milestone
My second milestone includes setting up the camera, running the required code, and testing the model. After plugging in the camera, I ran the command sudo raspi-config to go to the settings. Then I went to interface options and enabled legacy camera support. One of the challenges I faced was trying to test the camera because I wasn't able to test it due to the terminal window saying that there was an error with no camera detected, but towards the end when I needed the live video feed, the camera was detected. After I set up the camera, I entered the directory in which the pre-trained model was located and ran the model. After the model ran, a new popup window opened with the live video feed from the Arducam. I tested the model by putting objects such as a cellphone, a laptop, and a chair in front of the camera, and it correctly detected these objects. My next steps would be streamlining my model to detect a few certain objects and training the model by myself. 


<iframe width="560" height="315" src="https://www.youtube.com/embed/MZ-rnKBLxSw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


# First Milestone
My first milestone included setting up the raspberry pi 400 and the 1080p 8mp Arducam, as well as downloading the required software and libraries to carry out the model. First I placed an SD card into my laptop, to download the software required for the raspberry pi 400 to run onto the sd card. I had to use a microSD to SD card converter to place the SD card in my laptop because the Pi 400 only has a slot for a microSD card and not for an SD Card.  Then I plugged in the micro HDMI to HDMI Cable to the USB Capture card, which is plugged into my laptop. The function of the capture card is to allow the audio and video of the raspberry pi to be streamed to my laptop. I am using OBS Studio as the software to which the audio and video of the raspberry pi will be streamed. I set up my camera by plugging in the USB cable into the raspberry pi, and the connector into the camera. Then I plugged in my Canakit USB-C power supply to my raspberry pi and my outlet, which allowed for my Pi 400 to be powered on. After this, I had to plug in an external mouse to the Pi 400 because the laptop's keyboard and mouse don't work with the Pi (the keyboard is already built into the Pi 400, so no necessity for an external keyboard). 

The required downloads for my model include downloading open cv, TensorFlow light, and a pre-trained model to use. I used a pre-trained model instead of training my model because training my model would require tens of thousands of pictures. I used TensorFlow light instead of Tensorflow because Tensorflow lite is tuned more towards devices with lower power such as the Pi 400. I used an open cv to help with the object detection part and used the live video feed. After all the downloads, I cloned the repository with the pre-trained model to save it on my local raspberry pi. After this, I set up a virtual environment to make sure that each library has its separate space so that the downloaded libraries do not interfere with other projects or environments on the Pi. My next plan is to run the required files and code, set up the camera, and test the model.  


<iframe width="560" height="315" src="https://www.youtube.com/embed/5RkA6z8jvus" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


<!---# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 
-->

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```python
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts of your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Raspberry Pi 400 | The device on which the code and the model are run on | $98.00 | <a href="https://www.amazon.com/Raspberry-400-Computer-Kit-RPI400-US/dp/B08MYVQW1S/ref=sr_1_3?crid=13YPAIJE5PFCE&keywords=raspberry+pi+400&qid=1687277135&sprefix=raspberry+pi+400%2Caps%2C148&sr=8-3"> Link </a> |
|:--:|:--:|:--:|:--:|
| Logitech M185 | External Mouse which works with the raspberry pi | $11.99 | <a href="https://www.amazon.com/Logitech-M185-Wireless-Mouse-910-003888/dp/B004YAVF8I/ref=sr_1_4?crid=2YYMS9DE0VR3Q&keywords=logitech%2Bm185&qid=1687277254&sprefix=logitech%2Bm185%2Caps%2C146&sr=8-4&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Arducam 8MP 1080P USB Camera Module for Raspberry Pi | Gives the live video feed where the objects are detected | $30.00 | <a href="https://www.amazon.com/Arducam-Camera-Raspberry-Windows-Android/dp/B07YHK63DS/ref=sr_1_1_sspa?crid=3NROKHUG4NWP6&keywords=Arducam+8MP+1080P+USB+Camera+Module+for+Raspberry+Pi&qid=1687967026&sprefix=%2Caps%2C402&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| 4k HDMI Video Capture Card | Used to help display the Raspberry Pi on OBS Studio, and allows to use my laptop as a monitor  | $15.99 | <a href="https://www.amazon.com/LinkBand-Capture-Camcorder-Streaming-Nintendo/dp/B089ZWX5MY/ref=sr_1_4?keywords=4k+hdmi+video+capture+card&qid=1687967102&sprefix=4k+HDMI+Vide%2Caps%2C169&sr=8-4"> Link </a> |
|:--:|:--:|:--:|:--:|
| Canakit USB C Power Supply | Supplies power to the raspberry pi | $10.99 | <a href="https://www.amazon.com/CanaKit-Raspberry-Power-Supply-PiSwitch/dp/B07TSFYXBC/ref=sr_1_4?crid=3KPZ6OSQILGUA&keywords=canakit+usb+c+power+supply&qid=1687967332&sprefix=canakit+usb+c+power+supply%2Caps%2C142&sr=8-4"> Link  </a> |
|:--:|:--:|:--:|:--:|
| 64 GB micro SDcard to SD Card adapter | storage device to store the downloaded Raspberry Pi os, and allows for the software to be used on the Raspberry Pi 400  | $6.99 | <a href="https://www.amazon.com/Micro-Center-Class-Memory-Adapter/dp/B07YLZ8D1Y/ref=sr_1_10?crid=16R1RHOD1IKYU&keywords=micro%2Bcenter%2Bmicrosd%2B64gb%2Bwith%2Bsd%2Bcard%2Bconverter&qid=1687967985&sprefix=micro%2Bcenter%2Bmcrosd%2B64gb%2Bwith%2Bsd%2Bcard%2Bconverte%2Caps%2C158&sr=8-10&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| MicroHDMI to HDMI Cable | Connects Raspberry Pi 400 to HDMI Capture card, to display raspberry pi content on laptop[  | $8.99 | <a href="https://www.amazon.com/UGREEN-Adapter-Ethernet-Compatible-Raspberry/dp/B06WWQ7KLV/ref=sr_1_1_sspa?keywords=micro+hdmi+to+hdmi+cable&qid=1687972548&sprefix=microhdmi+t%2Caps%2C231&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1"> Link </a> |
|:--:|:--:|:--:|:--:|


# Starter Project
For My starter Project, I made the Simon Says Game. The game works by following a pattern which is displayed by the game, in the correct order. If the order is not followed, or if any button is not pressed, the user automatically loses, and the game restarts. The components used include a microcontroller, a buzzer, capacitors, a resistor, LEDs, slide switches, battery clips, batteries, a button pad and bezels, Standoffs and screws, and a PCB Board. First, I soldered the capacitors, the resistor, the microcontroller, and the buzzer to the bottom of the board. Then I turned over the board and soldered on the battery clips, LEDs, and slide switches. After that, I had to screw in the button pad and the bezel using screws and standoffs and placed the batteries into the battery holders. then my game was completed. One challenge which I faced while making the game included the game not responding to any presses by the user. I tried to clean the board, and where the wiring which completes the circuit is, but that didn't work, causing me to restart, but allowing me to finish the game quicker.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4YJrs3cAs38" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
