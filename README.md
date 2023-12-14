# pstnSPAMguard - Putting an End to Unwanted Calls

Are relentless SPAM calls driving you crazy? Does answering robocalls make you want to scream? pstnSPAMguard is a savvy method designed to cut down on those automated intrusions.

In my quest to reclaim phone serenity, I decided to harness the power of a Digital Receptionist, also known as IVR (Interactive Voice Response), to sift through the SPAM calls plaguing my line.

I use Voip.ms as my host for the phone number but this method should work on other self-managed VOIP providers too.

The first step involved uploading audio files ready to be deployed by the IVR system. The welcoming voice on the opening recording politely states, "Thank you for calling this number. If you are a human, please press one." A simple instruction, but a human touch is required to proceed; otherwise, the call is assumed to be SPAM and disconnected.

Following this, a confirmation recording reassuringly utters, "Connecting your call," serving as confirmation that the correct button was indeed pressed.

## How To

First I needed to upload some audio files that the IVR system will use when accessed by a caller to my number 

![1](https://github.com/evdelen/pstnSPAMguard/assets/373773/bffd104d-e1eb-4491-b4b1-b699a9ab51a3)

I called my IVR "Human Check". 

It plays the first audio recording then provides 5 seconds for the user to respond. From there we hae 3 bnaches:

- 1 is pressed then you can connect the call directly or connect to a second IVR that plays the confirmation that then connects the call.
- 'i' is the option for an invalid key. You can hangup the call or connect to a "try again" IVR.
- 't' is the option for a timeout. If no key is pressed then you can hangup the call or connect to a "try again" IVR.

![2](https://github.com/evdelen/pstnSPAMguard/assets/373773/6dff97e6-1baa-4f69-b502-5bd0ebe92055)
