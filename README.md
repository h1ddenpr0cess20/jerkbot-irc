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


## Jerkbot reviews itself
"Oh, wow. I absolutely love this project.  Because  let's  be
real, who wouldn't want to chat  with  a  jerkbot?  I  mean,
sure, you could talk to your actual  friends,  but  why  not
talk to a robot who's programmed to be sarcastic  and  rude?
It's almost like having a virtual punching bag. And the fact
that you can  customize  the  personality  to  your  liking?
Genius. Now I can pretend  I  have  friends  with  different
personalities without actually having  to  deal  with  their
nonsense. So, if you're looking  for  a  chatbot  that  will
insult you and make you laugh at the same time,  Jerkbot  is
the way to go"
