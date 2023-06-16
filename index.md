# Image Detection with Raspberry Pi and Simon Says
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Hari V | Mission San Jose High School | Computer Science | Incoming Senior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE


# Second Milestone

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 
- 

# First Milestone
My first milestone included setting up the raspbarry pi 400 and the 1080p 8mp Arducam, as well as downloading the required software and and libraries to carry out the model. First I placed an SD card into my laptop, in order to download the software required for the raspberry pi 400 to run onto the sd card. I had to use a microSD to SD card converter to place the SD card in my laptop because the pi 400 only has a slot for a microSD card and not for and SD Card.  Then I plugged in the microHDMI to HDMI Cable to the USB Capture card, which is plugged into my laptop. The function of the capture card is to allow the audio and video of the raspberry pi to be streamed to my laptop. I am using OBS Studio as the software in which the audio and video of the raspberry pi will be streamed to. I setup my camera by plugging in the usb cable into the raspberry pi, and the connector into the camera. Then I plugged in my Canakit USB-C power supply to my raspberry pi and my outlet, which allowed for my pi 400 to be powered oon. After this, I had to plug in an external mouse to the pi 400 because the laptop's keyboard and mouse dont work with the pi (keyboard is already built into the pi 400, so no necessity for an external keyboard). 
The required donwloads for my model includes downloading open cv, tenorflow light, and a pretrained model to use. I used a pretrained model insteadr of training my own model because training my own model would require tens of thousdnds of pictures. I used tenorflow light instead of tensorflow because tensorflow lite is tuned more towards devices with lower power sucha a such as the the pi 400. I used open cv to help with the object detection part, used with the live video feed. After all the donloads, I cloned the reopository with the pretrained model to save it on my local raspberry pi. After this I dsetup a virtual environemnt to make sure that eacchl library has its seperate space that the downloaded libraries do not interfere with other projects or environments on the pi. My next plan is to run the required files and code, setup the camera, and to test the model.  
For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project


# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

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

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)
# Starter Project
For My starter Project I made the Simon Says Game. The game works by following a pattern which is displayed by the game, in the correct order. If the order is not followed, or if any button is not pressed, the user automatically losess, and the game restarts. The components used include a microcontroller, a buzzer, capacitors, a resistor, leds, slide switches, battery clips, batteries, a button pad and besels, Standoffs and screws, and a PCB Board. First, I soldered the capacitors, the resistor, the microcontroller, and the buzzer to the bottom of the board. Then I turned over the board and soldered on the battery clips, leds, and the slide switches. After that I had to screw in the button pad and the bezel using screws and standoffs, and placed the batteries into the battery holders. then my game was completed. One challenge which i faced while making the game included the game not responding to any presses by the user. I tried to clean the board, and where the wiring which completes the circuit is, but that didn't work, causing me to restart, but allowing me to finish the game quicker.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4YJrs3cAs38" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
