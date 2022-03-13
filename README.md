# CS420X-Final
[Video](https://youtu.be/Z5hxwZ-ZOMU)
[Link](https://evelyntrvn.github.io/CS420X-Final/)

For this project, it took me a while to figure out what I could do in the time that I had. I first played around with a couple of other simulations such as the fluid simulation but figured given my time frame, I would continue with my A3 project for the diffusion-reaction simulation. At first, I played around with video input but was not able to figure out how to implement it with the current textureback and texturefront. Because of this, I started to look at how audio input could impact the simulation.

Trying to figure out the best way to send the audio data to the GPU honestly took a large amount of time for me. I had started with playing around with the microphone as an input. I was able to get the audio data, however, the data itself was in an array. I eventually instead took the average of that given array because there were a lot of zeros for any silence in my speech. In addition to that, I also needed to implement a mapping function because the audio controlled the kill variable. If the kill variable was too low or too high, the whole simulation would disappear before it even started. In addition to that, with just the microphone input, it didn’t serve as a very consistent visual nor the best-looking one. As a result, I added pre-loaded songs to use instead. 

In addition to that, I used the audio to change the amount of blue and attempted to add a glow throughout the whole visual as a post-processing effect. In my honest opinion, while I am proud of what I’ve done with the given time, I wish I could do more. One thing I would want to fix with my current project is the shine causes the green to start to seep from the right side. It does look interesting at times, but I do recognize that it can also look messy. Some other future implementation ideas I have include, having the audio frequency change the speed at which the simulation goes and also having multiple reactions overlap one another, each based on a different color.

Song Credits: Marble Soda by Shawn Wasabi, Burnt Rice by Shawn Wasabi, Lacrimosa by Mozart
