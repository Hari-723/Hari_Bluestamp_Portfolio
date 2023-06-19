# Object Detection with Raspberry Pi and Simon Says
<!---Replace_this_text_with_a_brief_description_(2-3 sentences)_of_your_project._This_description_should_draw_the_reader_in_and_make_them_interested_in_what you've_built._You_can_include_what_the_biggest_hallenges,_takeaways,_and_triumphs_from_completing_the_project_were._As_you_complete_your_portfolio, remember your_audience_is_less_familiar_than_you_are_with_all_that_your_project_entails!-->

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Hari V | Mission San Jose High School | Computer Science | Incoming Senior

<!--**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**--->

![Headstone Image](logo.svg)
  
# Final Milestone
<!---For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE-->


# Second Milestone
My second milestone includes setting up the camera, running the required code, and testing the model. After plugging in the camera, I ran the command sudo raspi-config to go to the settings. Then I went to interface options and enabled legacy camera support. One of the challenges I faced was trying to test the camera because I wasn't able to test it due to the terminal window saying that there was an error with no camera detected, but towards the end when I needed the live video feed, the camera was detected. After I set up the camera, I entered the directory in which the pre-trained model was located and ran the model. After the model ran, a new popup window opened with the live video feed from the Arducam. I tested the model by putting objects such as a cellphone, a laptop, and a chair in front of the camera, and it correctly detected these objects. My next steps would be streamlining my model to detect a few certain objects and training the model by myself. 
<!---For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone -->
- 

# First Milestone
My first milestone included setting up the raspberry pi 400 and the 1080p 8mp Arducam, as well as downloading the required software and libraries to carry out the model. First I placed an SD card into my laptop, to download the software required for the raspberry pi 400 to run onto the sd card. I had to use a microSD to SD card converter to place the SD card in my laptop because the Pi 400 only has a slot for a microSD card and not for an SD Card.  Then I plugged in the micro HDMI to HDMI Cable to the USB Capture card, which is plugged into my laptop. The function of the capture card is to allow the audio and video of the raspberry pi to be streamed to my laptop. I am using OBS Studio as the software to which the audio and video of the raspberry pi will be streamed. I set up my camera by plugging in the USB cable into the raspberry pi, and the connector into the camera. Then I plugged in my Canakit USB-C power supply to my raspberry pi and my outlet, which allowed for my Pi 400 to be powered on. After this, I had to plug in an external mouse to the Pi 400 because the laptop's keyboard and mouse don't work with the Pi (the keyboard is already built into the Pi 400, so no necessity for an external keyboard). 

The required downloads for my model include downloading open cv, TensorFlow light, and a pre-trained model to use. I used a pre-trained model instead of training my model because training my model would require tens of thousands of pictures. I used TensorFlow light instead of Tensorflow because Tensorflow lite is tuned more towards devices with lower power such as the Pi 400. I used an open cv to help with the object detection part and used the live video feed. After all the downloads, I cloned the repository with the pre-trained model to save it on my local raspberry pi. After this, I set up a virtual environment to make sure that each library has its separate space so that the downloaded libraries do not interfere with other projects or environments on the Pi. My next plan is to run the required files and code, set up the camera, and test the model.  
<!---
For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project
-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/5RkA6z8jvus" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


<!---# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 
-->
<!---
# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```
-->
<!---# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|-->


# Starter Project
For My starter Project, I made the Simon Says Game. The game works by following a pattern which is displayed by the game, in the correct order. If the order is not followed, or if any button is not pressed, the user automatically loses, and the game restarts. The components used include a microcontroller, a buzzer, capacitors, a resistor, LEDs, slide switches, battery clips, batteries, a button pad and bezels, Standoffs and screws, and a PCB Board. First, I soldered the capacitors, the resistor, the microcontroller, and the buzzer to the bottom of the board. Then I turned over the board and soldered on the battery clips, LEDs, and slide switches. After that, I had to screw in the button pad and the bezel using screws and standoffs and placed the batteries into the battery holders. then my game was completed. One challenge which I faced while making the game included the game not responding to any presses by the user. I tried to clean the board, and where the wiring which completes the circuit is, but that didn't work, causing me to restart, but allowing me to finish the game quicker.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4YJrs3cAs38" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
