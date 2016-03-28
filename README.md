# Universal Windows App - Speech Translate Demo

The goal of this demo is to demonstrate the use of the UWP audiograph library and integrate with the Microsoft Translator Speech Translate API.  The demo takes input audio bytes from audio input (ex. microphone) and send the translated text to voice output to the audio output (ex. speaker).  The demo app shows

## Key Features
1. Use HttpClient to retrieve an Azure Marketplace Token with the Client Id and Client Secret.
2. Populate a dropdown list with the set of languages that we support for speech translate - https://dev.microsofttranslator.com/languages
3. Use Websocket library to communicate with the speech translate api - https://dev.microsofttranslator.com/speech/translate
4. Connect the AudioGraph library and demonstrate converting IEEE Float (output from the AudioGraph) to 16bit PCM for input to the speech translate API.

## Usage
Visual Studio 2015+ with Windows 10
Make sure the Universal Windows App development feature is enabled in Visual Studio

## Settings
Subscribe to the Microsoft Speech Translate offering and enter your credentials in
MainPage.AzureDataMarketClientId and MainPage.AzureDataMarketClientSecret

## References
UWP Audiograph and Websocket references
http://mtaulty.com/2016/02/09/windows-10-uwp-audiographrecording-microphone-to-wav-file/
https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/AudioCreation
https://msdn.microsoft.com/en-us/library/windows/apps/windows.media.audio.audiograph.aspx
https://msdn.microsoft.com/en-us/windows/uwp/audio-video-camera/audio-graphs
https://msdn.microsoft.com/en-us/windows/uwp/networking/websockets


