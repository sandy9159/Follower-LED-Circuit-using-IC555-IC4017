# Follower-LED-Circuit-using-IC555-IC4017



![image](https://user-images.githubusercontent.com/19898602/141060395-bf677e26-b847-48d5-9800-b2e6bd2a6b66.png)
  
  
  In this tutorial i will show you how to make simple a LED Chaser or Sequencer using 555 & 4017 circuit. 
  
  You can watch the video which is embedded in this step for construction, 
  
  parts list, circuit diagram & testing or you can continue reading the post for further details.
  
  A simple LED chaser hobby circuit can be made using 555 timer and CD4017 counter IC. 
  
  You can use this circuit for decorative purposes. By modifying the circuit in a proper way, 
  
  you can even use this to control lights working on AC mains.
  
  # COMPONENT LIST
  
>  1 * 555 

> 1 * 4017 

> 1 * 8 Pin IC Base 

> 1 * 16 Pin IC Base 

> 5 each * Blue & Green LED 

> 1 * 2 Pin Terminal Block 

> 2 * 1.5k Ohm

> 1 * 0.01uF

> 1 * 4.7uF/50V

> 1 * 10k Pot wires 


# IC 555

![image](https://user-images.githubusercontent.com/19898602/149891001-0fc617b9-78bb-492d-bd8d-5703d2c4eb6a.png)


We have seen that Multivibrators and CMOS Oscillators can be easily constructed from discrete components to produce relaxation oscillators for generating basic square wave output waveforms. But there are also dedicated IC’s especially 

designed to accurately produce the required output waveform with the addition of just a few extra timing components.

One such device that has been around since the early days of IC’s and has itself become something of an industry “standard” is the 555 Timer Oscillator which is more commonly called the “555 Timer”.

The basic 555 timer gets its name from the fact that there are three internally connected 5kΩ resistors which it uses to generate the two comparators reference voltages. 

The 555 timer IC is a very cheap, popular and useful precision timing device which can act as either a simple timer to generate single pulses or long time delays, or as a relaxation oscillator producing a string of stabilised waveforms of varying duty cycles from 50 to 100%.

![image](https://user-images.githubusercontent.com/19898602/149890834-d12ceff0-b00a-4e63-894a-c2b8e9a709ab.png)

![image](https://user-images.githubusercontent.com/19898602/149890889-68b03715-9d1f-4362-a5b3-91b35f8aeb8b.png)

# IC 4017

![image](https://user-images.githubusercontent.com/19898602/149891183-bb1c69b3-2e6e-44f0-bf89-aeab9e527f20.png)

CD4017 or HCF4017BE or 74HC4017 is a CMOS decade counter/ Divider. It has 16 pins and this counter has 10 decoded outputs.  

This is known also as 10 stages ‘Johnson decade counter.  It has total 10 outputs. when a clock signal from the clock input given 

then output turns to Highl one by one in sequence. When the clock input is given to input, at each pulse of the clock input signal the output turns on in sequence.

CD4017 is the most popular ic which is widely used in various applications like Binary counter, Decoder, Decade counter, Frequency division, etc. 

This is more useful in different types of projects like Light Chaser, Remote controlled Switch, Alarm, Touch ON-OFF  switch, Clap switch, Matrix Die etc.




![image](https://user-images.githubusercontent.com/19898602/149891420-4b9fead9-f321-45fd-936a-8e6d8d745105.png)


#  CIRCUIT DIAGRAM AND PCB DETAILS

![image](https://user-images.githubusercontent.com/19898602/141062055-e9f6e404-a53a-491a-adfe-304eb1c7a9f7.png)

Construct the circuit as shown in the circuit diagram.

For making the LED Chaser you require 555 Timer & 4017 Counter. The 555 Timer is used to produce the clock pluse for the 4017. The 4017 is constructed in a Astable configuration.

When the clock pulse produced by the 555 timer is fed to the 4017, it starts counting in the upward direction for each pulse. Now when you connect the LED's to the outputs you get the sequential glow.

The duration of the glow of led's can be altered by changing the value of pot (RV1) & the value of C2 Capacitor. or only by changing the value of pot (RV1).

![image](https://user-images.githubusercontent.com/19898602/141062382-0819ee2b-937e-4119-8f55-4a9ca0f4d99d.png)
![image](https://user-images.githubusercontent.com/19898602/141062423-9db2b854-c1d8-4a00-8077-bdf87100fb78.png)


In the circuit diagram i showed the circuit which counts upto the value 10. You can change the value of count by simply connecting the last sequence to the reset pin. For example

Let say you want the count to be 6
Then you need to connect the Q0 to Q5 to the LED's & the Q6 to the Reset Pin 15.
Remaining pins from Q7 to Q9 will be No Connection.

![image](https://user-images.githubusercontent.com/19898602/141063331-f61b3938-40ce-4e22-8ba7-7e1550a2d39c.png)
![image](https://user-images.githubusercontent.com/19898602/141063382-a7b48761-2c2f-4bfb-a49e-d2cfdeb4fde8.png)

I have ordered PCB from [JLCPCB](https://jlcpcb.com/IAT )

This is the link of [PCB editabl file](https://oshwlab.com/sharmaz747/multipurpose-pcb)

If you seriously need quality PCB quickly in your hand then you must have to try [JLCPCB](https://jlcpcb.com/IAT ) PCB manufacturing service.
They have Special offer of $2 for 1-4 Layer PCBs, free SMT assembly monthly.
If new user signup today from this link [JLCPCB](https://jlcpcb.com/IAT ) you will get 30$ coupon from [JLCPCB](https://jlcpcb.com/IAT ).

You can easily understand the working of the circuit from the above animation. As I explained above, 555 timer is wired as an astable multivibrator. 

Please read the article Astable Multivibrator using 555 Timer for detailed explanation. So the 555 will 

produce square wave output and which will act as a clock for the CD4017 counter IC.

You can see that for each high pulse output of 555, the output of 4017 is incrementing by one. Output frequency of 

555 astable is given by the following equation.

Output Frequency =  1.44/((R1 + 2RV1) * C1)
So you can easily change the output frequency of above circuit by varying the preset RV1. By this we can change the LED chasing speed.

![image](https://user-images.githubusercontent.com/19898602/141063631-00b80017-3a14-4f6e-8667-e8f319461847.png)
![image](https://user-images.githubusercontent.com/19898602/141063700-9e80d188-2150-4fbb-83cb-11e2e995e55e.png)


![MVI_0004](https://user-images.githubusercontent.com/19898602/141063951-8fdeff03-6cbe-4f56-8d6e-584a75bb80e4.gif)


