# pstnSPAMguard
A method to reduce SPAM phone calls.

I got tired of getting automated SPAM marketing calls so I setup a Digital Receptionist or IVR - Interactive Voice Response - to screen SPAM calls.

I use Voip.ms to host my phone number but similar systems can be setup on any service.

First I needed to upload some audio files that the IVR system will use when accessed by a caller to my number 

The opening audio recording says "Thank you for calling this number. If you are a human please press one." At that point a human is expected to press one while a SPAM call will just play their own audio.

The confirmation recording says "Connecting your call" and is used for a confirmation that the correct button was pressed.

I created an IVR that I called "Human Check" that plays the opening recording. Then the caller is given a five second timeout to press one to connect the call.

From there you define the different possible routes:
- 1 is pressed then you can connect the call directly or connect to a second IVR that plays the confirmation that then connects the call.
- 'i' is the option for an invalid key. You can hangup the call or connect to a "try again" IVR.
- 't' is the option for a timeout. If no key is pressed then you can hangup the call or connect to a "try again" IVR.
