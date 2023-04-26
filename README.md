# jerkbot-irc
Jerkbot is an OpenAI chatbot for IRC (Internet Relay Chat).  It is named for the sarcastic jerk personality I use for my instance.  You can set any default personality you would like.  It can be changed at any time, and each user has their own separate chat history with their chosen personality setting.  Users can interact with each others chat histories for collaboration if they would like, but otherwise, conversations are separated.

## Installation

```
pip3 install openai irc
```
Get an [OpenAI API](https://platform.openai.com/signup) key 

Fill in the variables for channel, nickname, password and server in ircBotLauncher.py.  
Password is optional, but registration is required for some channels.

## Use
```
python3 ircBotLauncher.py
```
**.ai _message_ or botname: _message_**
    Basic usage.
    Personality is preset by bot operator.
    
**.x _user message_**
    This allows you to talk to another user's chat history.
    _user_ is the display name of the user whose history you want to use
     
**.persona _personality_**
    Changes the personality.  It can be a character, personality type, object, idea.
    Don't use a custom prompt here.
    If you want to use a custom prompt, use .stock then use .ai _custom prompt_
        
**.reset**
    Reset to preset personality
    
**.stock**
    Remove personality and reset to standard GPT settings

**.help _botname_**
    Display the help menu

## Screenshots
### Default personality
![image](https://user-images.githubusercontent.com/127710567/234454514-9084e364-c495-41e5-807b-ae965f180cd5.png)

### Persona feature
![image](https://user-images.githubusercontent.com/127710567/234455016-71a4cba9-7dfa-4724-9898-a0b07fe146d0.png)

![image](https://user-images.githubusercontent.com/127710567/234456412-e3a34f6a-a6d4-4fa4-b7e3-c17acebe2205.png)

