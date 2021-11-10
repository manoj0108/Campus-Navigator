# Campus-Navigator

Campus navigator is a Navigation system that can work even in the absence of GPS connectivity. The system will have a hand-held device that automatically locates the user location and updates it to the user. Based on the destination inputs given by the user, the system determines the shortest path to the desired destination of the user.

There will be navigators at some points inside the campus, but users do not have continuous help to get to their destination. They can try to figure out a way to get to their
target destination as per the navigators available in the campus. However when they start walking towards their target direction, they have no help anymore and face many
problems. The campus navigator will help in overcoming these problems and provide efficient path to the desired destination.

![Screenshot 2021-11-10 122809](https://user-images.githubusercontent.com/69961625/141065072-80419ee8-2834-4b95-b57a-eb9d29e5d049.png)

The system is mainly based on the transmission of the data between the RF transceiver modules. The encoder integrated circuit (IC) is coded with the data bits which has the
location information of the transmitting building or block. The IC generates series of bits which has both security bits and the data bits. These series of bits are continuously
transmitted by the RF transmitters placed at every block in the campus. The user has to carry the RF receiver module with him. When the RF receiver module comes in the range
of the transmitter signals, the code encoded in that signal is decoded by the decoder IC and sent to the Arduino board. The Arduino board processes the data bits received and
the user location which is decoded will be displayed over the LCD screen.The receiver module with the user then asks for the destination location information in the form of digits. Based on the current location and user input on the destination, the Arduino board estimates the shortest path to the destination. This information is displayed on the LCD screen.
