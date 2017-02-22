# Controller Section 

I choose iPhone6 to control the car. So, I used the ios simulink hardware suport package to create this file.
Note that you need xcode7 and iPhone in ios9.3 only and you need to setup first.   

<img width="1032" alt="screen shot 2560-02-22 at 6 20 18 pm" src="https://cloud.githubusercontent.com/assets/9088660/23209374/9f4aa63a-f92b-11e6-8fda-ee0420848811.png">

## Block Configuration
There are 3 types of Simulink in this model.
  1. Slider : DC Motor, Servo
  2. Button : Emergency, Forword or Reverse
  3. Display
  4. UDP send 

### For slider block
You need to set the minimum, the maximum and the middle value of the slider. You need to set the sample time and the resolution which is the step of the slider.   

<img width="566" alt="screen shot 2560-02-22 at 6 29 12 pm" src="https://cloud.githubusercontent.com/assets/9088660/23209702/df07a5b0-f92c-11e6-8d5b-4e309b8dd797.png">

### For UDP send block
You need to set your target remote IP address and remote IP port.

<img width="395" alt="screen shot 2560-02-22 at 6 32 31 pm" src="https://cloud.githubusercontent.com/assets/9088660/23209806/61b3e7d0-f92d-11e6-9fec-25198c47fa11.png">

### For Button block
You need to set button state and the sample time. 

<img width="399" alt="screen shot 2560-02-22 at 6 49 48 pm" src="https://cloud.githubusercontent.com/assets/9088660/23210352/c9f2ef7e-f92f-11e6-87bd-07809646f8ad.png">


After finishing seting  all block then deploy to the hardware.
