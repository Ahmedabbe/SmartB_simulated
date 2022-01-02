###### *SmartB_simulated*
###### *(This iteration uses simulated data in Node Red)*

## Background

This project is a sort of proof of concept for creating an affordable hive monitoring system for private use.

The idea is to give the beekeeper more insights into the state of each individual hive while minimizing the need to open said hives up for possibly disruptive manual inspections. This is especially useful in colder places or during harsh winters when opening a hive exposes the bees to potentially lethal temperatures. 

Let's look at what combination of data is relevant for a beekeeper and what information about the hive might be gleaned from said data. 

- Temperature and humidity:  
  Although bees generally don't need help managing the internal temp or humidity of a hive, it's still useful data for figuring out how well a particular colony is     doing. For example, by establishing a baseline temp, a beekeeper can infer about how the queen is faring or if there is enough food by monitoring temperature         fluctuations. Keeping optimal humidity levels equally play an important roll in, amongst other things, honey production and prevention of harmful fungal growths. 
  
- Noise levels:   
  Keeping an eye on the amount sound a colony is emitting is very helpful in determining how "agitated" the bees are. This is most noticable when the colony is         queenless or disburbed by an animal. During these events decibel levels can go upwards of 80-90db. 
  
Monitoring weight of the entire hive would also be very useful, particularly during honey production. You wouldn't have to manually inspect each hive as often. This   is something that I want to try and look at in the future after getting these internal systems set up.
   
## System overview 


![Untitled Diagram drawio(1)](https://user-images.githubusercontent.com/70702026/147887574-a8469d3a-e7fa-4253-92b5-361ceb5809f0.png)

*Node Red flow:*
![Screenshot 2022-01-01 at 14-33-06 Node-RED](https://user-images.githubusercontent.com/70702026/147887589-47143b46-885a-4f55-a25c-c6869e3e806e.png)


### Tech hardware 
*Materials used in the current simple prototype*
- DHT22 sensor (temp and humidity)
- LMV324 (audio)
- RFM95W (LoRaWAN transmitter)
- ESP32 (LoRaWan receiver/WiFi module)

### 
