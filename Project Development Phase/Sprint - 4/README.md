COPYING CREDENTIALS FOR API AND URL:
 
 
  ![image](https://user-images.githubusercontent.com/115462847/202408536-684c3bac-07a7-44c2-a7a3-35f448c51b76.png)




PROGRAM FOR ACCESSING APIs OF TTS SERVICE:

from ibm_watson import TextToSpeechV1
from ibm_cloud_sdk_core.authenticators import IAMAuthenticator
authenticator = IAMAuthenticator('1SuMpBioLx9PuvKX- wnvMh3Z3lQbUKcXZErWleXdmY9j')
text_to_speech = TextToSpeechV1( authenticator=authenticator
)
text_to_speech.set_service_url('https://api.au-syd.text-to- speech.watson.cloud.ibm.com/instances/d3e4f1ee-ccf4-4e79-a3bf-71cdb9fdf9e8')
with open('hello_world.wav', 'wb') as audio_file: audio_file.write(
text_to_speech.synthesize( 'Take Crocin Now',
voice='en-US_AllisonV3Voice', accept='audio/wav'
).get_result().content)




EXECUTE THE RUN:

![image](https://user-images.githubusercontent.com/115462847/202409032-36aec95b-d405-441d-ae65-34c9d5c2f407.png)



DATAS SEND FROM NODE UI TO MIT APP 

![image](https://user-images.githubusercontent.com/115462847/202412380-b1d05c1d-f444-459b-9a12-6ace35fc2164.png)




TEXT TO SPEECH - IN MIT APP:

![image](https://user-images.githubusercontent.com/115462847/202411324-0bdeef90-366f-4e2d-86cf-426d3846d890.png)




