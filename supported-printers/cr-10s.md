# CR-10S

This guide will go through the process of hooking up your QuadFusion to Creality's CR-10S printer.

{% hint style="warning" %}
The QuadFusion and the company M3D have no affiliation with the CR-10S or its company.
{% endhint %}

### Mechanically









### Electrically

{% hint style="info" %}
You will need a Duet Maestro board if you with to follow along during the electrical part of this guide. Look at the bottom of the page to see where to get one.
{% endhint %}

This is the Duet Maestro:

![https://duet3d.dozuki.com/Wiki/Duet\_2\_Maestro\_Hardware\_Overview](../.gitbook/assets/image%20%2832%29.png)

This will be a walk through on how we hooked up the QuadFusion, as well as part of the CR-10S, to the Duet Maestro board.

Before you can begin to wire your QuadFusion to the Duet Maestro board you must attach an extension to the board. With this extension you will be able to connect the the extra motor wires to the board.

The following pictures show where the extension goes, and how it looks once it has been plugged in: 

![](../.gitbook/assets/image%20%2852%29.png)

![](../.gitbook/assets/image%20%282%29.png)

### Base Connections

![](../.gitbook/assets/image%20%285%29.png)

Without the fans, the QuadFusion has six main wires coming from it. The four wires with yellow dots at the ends are the motor wires. The wire with a green dot is the heater wire, and lastly the wire with the red dot is the PT1000 \(or thermistor\). 

The wires plug in to their corresponding color that is boxed in the following picture:

![](../.gitbook/assets/image%20%2838%29.png)

Notes:

* Keep in mind when you're wiring your QuadFusion's motors to the Duet Maestro board which motor is connected to which port. The first picture in this guide labels each port as E0 Stepper, E1 Stepper, E2 External Driver, and E3 External Driver. When facing the front of your QuadFusion, the front left motor is 0, the front right motor is 2, the back left motor is 1, and the back right motor is 3. 
* If you decide to extend the wires given to you, make sure that you are maintaining the original positive and negative wires. 

The next steps will be to connect your CR-10S' stepper motors, power source, and Z-probe

{% hint style="warning" %}
The CR-10S we worked with used a Z-probe instead of the Z-limit switch the printer came with. Additionally, we ended up having the bed heated separately, which will be explained within the guide.  
{% endhint %}


