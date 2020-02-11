# socketChannel_RasaBot
Bot for testing the usage of Rasa webchat


**Step1**: Just add the `socketChannel.py` file from this repository to your project : 

> https://github.com/JiteshGaikwad/socketChannel_RasaBot/blob/master/socketChannel.py

**Step2**: Now register the above channel in your `credentials.py` file as mentioned in this repo:

>https://github.com/JiteshGaikwad/socketChannel_RasaBot/blob/cae5b9c314238dfd927634f66b9a5c2a962bd662/credentials.yml#L19

**Step3**: Now in the bot-ui i.e `rasa-webchat`, add the customData that you want to send as mentioned here:

> https://github.com/botfront/rasa-webchat#in-a-script-tag

**Step4**: Now if you want to extract the `customData`, just write down the below code in your actions.py file:

>https://github.com/JiteshGaikwad/socketChannel_RasaBot/blob/cae5b9c314238dfd927634f66b9a5c2a962bd662/actions.py#L35

I have written the function that extracts the metadata from the tracker, you can get it here: 

>https://github.com/JiteshGaikwad/socketChannel_RasaBot/blob/cae5b9c314238dfd927634f66b9a5c2a962bd662/actions.py#L17

**Note**: I have just updated the `socket.io` channel's `handle_message` method to extract the `customData` as `metadata` : 
>https://github.com/JiteshGaikwad/socketChannel_RasaBot/blob/cae5b9c314238dfd927634f66b9a5c2a962bd662/socketChannel.py#L193
