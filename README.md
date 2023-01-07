There's no real-time way to get display msgs into home assistant via the TuyaMCU integration so my idea is to intercept the separate UART data stream from the MCU to the display. The tuya UART data stream is handled by the TuyaMCU component in ESPHome.

Decoding UART data streams is possible with ESPHome's abstraction layer and UART module. That gives you the data. Decoding it is probably going to be like deciphering encrypted German UBoat transmissions... hopefully easier.... time will tell. 

I used to work for Chevron way back in 1988. I was certified on a tool called a Lanalyzer which was a Compaq suitcase computer that weighed 50 lbs (and it had an 8088 CPU @ 8 mhz and an 8086 math coprossser). It was literally the very first Ethernet sniffer/protocol analyzer ever made. I was the most competent person in a company of 50,000 ppl that knew how to use it. This is bringing back ALL those nightmares of lugging it to Texas from CA and fixing network problems at 3am in a refinery telephone closet (worse than you can imagine).

That certainly helped me set up the config files for ESPHome and decipher the data stream.   There are lots of examples of doing this using TEXT.  But my data is in HEX.  And very few examples of it in action.  Hopefully this helps someone else.

Full breakdown  of getting this working is here: https://github.com/jazzmonger/uart-HEX-sniffer/discussions/1
