### Guardbot

A simple robot that looks around, chases faces and shoots.

### Instructions

#### Prerequisites

* *Lego NXT*
* *Android* `4.0`+
* Some Scala and Java knowledge

#### Build one!

*Guardbot, make II (2014)*

![Guardbot, make II](pics/make%20II%20-%201%20small.jpg)

*Guardbot, make I (2013)*

![Guardbot, make I](pics/make%20I%20-%201%20small.jpg)

We used tracked chassis, some collision detection sensors and a cannon or two. A couple of additional pictures can be found inside the [pics directory](https://github.com/stanch/guardbot/tree/master/pics).

#### How it works?

* The phone is the brain. It uses the camera to look for faces and sends the movement commands to the “body” via *Bluetooth*.
* The Lego part is the body. It mostly follows the commands from the brain, but also reacts to reflexes in case of collisions.

#### Installation

* Go to http://www.lejos.org/ and follow the instructions on how to flash your NXT brick.
* Pair your phone with the brick via Bluetooth.
* You may want to change the NXT dir [here](https://github.com/stanch/guardbot/blob/master/lejos/build.sbt#L8) (yeah, I know it’s ugly for now).
* Turn your brick on and connect to the PC. Then run

  ```
  cd lejos
  sbt upload
  ```
  
  This will upload the necessary code.
  
* Turn on your Android phone on and connect to the PC. Then run

  ```
  cd android
  sbt android:run
  ```
  
  This will upload and run the app on the phone.
  
#### Running

* Select the program on the brick and press “run”.
* Open the app on the phone and click “start”.
* There is no step 3!
  
#### Hacking



### Credits

Built and programmed by *Nuno Marques* and [*Nick*](http://github.com/stanch) in 2013 and yet again in 2014.
