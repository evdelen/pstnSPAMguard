# pstnSPAMguard
A method to reduce SPAM phone calls.

Tired of SPAM calls? I setup a Digital Receptionist or IVR - Interactive Voice Response - to screen SPAM calls.

I use Voip.ms to host my phone number but similar systems can be setup on any service.

I uploaded some audio files that the IVR system will use when accessed.

The opening audio recording says "Thank you for calling this number. If you are a human please press one." At that point a human is expected to press one while a SPAM call will just play their own audio.

The confirmation recording says "Connecting your call" and is used for a confirmation that the correct button was pressed.

I created an IVR called "Human Check" that plays the opening recording and pauses for 5 seconds. From there you define the different possible routes:
- 1 is pressed then you can connect the call directly or connect to a second IVR that plays the confirmation and then connects the call.
- 'i' is the option for an invalid key. You can hangup the call or connect to a "try again" IVR.
- 't' is the option for a timeout. If no key is pressed then you can hangup the call or connect to a "try again" IVR.
