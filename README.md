# Universal Windows App - Speech Translation API Demo

The goal of this example is to demonstrate the use of the UWP audiograph library and integrate with the Microsoft Translator Speech Translation API.  The demo takes input audio bytes from audio input (ex. microphone) and send the translated text to voice output to the audio output (ex. speaker).  The demo app shows:

1. Use HttpClient to retrieve an Azure Cognitive Services authentication token with a secret key from a subscription to the Speech Translation API.
2. Populate a dropdown list with the set of [languages supported for speech translation](http://docs.microsofttranslator.com/languages.html).
3. Use Websocket library to communicate with the [Speech Translation API](http://docs.microsofttranslator.com/speech-translate.html).
4. Connect the AudioGraph library and demonstrate converting IEEE Float (output from the AudioGraph) to 16 bit PCM for input to the Speech Translation API.

## Getting Started
Visual Studio 2015 or later, with Windows 10 is required. Make sure the Universal Windows App development feature is enabled in Visual Studio.

Subscribe to the Microsoft Translator [Speech Translation API](http://docs.microsofttranslator.com/speech-translate.html) offered in Microsoft Azure Cognitive Services. 

Retrieve your subscription key in the Azure developer portal. Enter your key in file `MainPage.xaml.cs`:

```
const string AzureSecretKey = "[Enter your Client Secret here]";
```

## References
UWP Audiograph and Websocket references
- http://mtaulty.com/2016/02/09/windows-10-uwp-audiographrecording-microphone-to-wav-file/
- https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/AudioCreation
- https://msdn.microsoft.com/en-us/library/windows/apps/windows.media.audio.audiograph.aspx
- https://msdn.microsoft.com/en-us/windows/uwp/audio-video-camera/audio-graphs
- https://msdn.microsoft.com/en-us/windows/uwp/networking/websockets



