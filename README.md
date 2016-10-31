# pivid
A collection of bash scripts to make viewing Twitch &amp; YouTube easier on a Raspberry Pi 3

## prerequisites
    apt-get install livestreamer youtube-dl

## configuration
edit the config file and put in your twitch api key. don't have one? get one here:

https://twitchapps.com/tmi/


## command examples
### twitch
Watch kripp in high quality...

    ./twitch/watch-high nl_kripp

Watch kripp in the best quality...

    ./twitch/watch-best nl_kripp

Watch league in 720p30
    
    ./twitch/watch-custom riotgames 720p30
    
See what modes are available to use with watch-custom.
  
    ./twitch/modes riotgames

### youtube
watch a video

    ./youtube/watch https://www.youtube.com/watch?v=h_NP7x35gd0

### notes
Your pi may not always be able to use the "best" feed. Further Twitch has been switching to more clearly defined quality levels such as 720p60 and 480p30. watch-custom allows you to specify which mode you want to watch.
