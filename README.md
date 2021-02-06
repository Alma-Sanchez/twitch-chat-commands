# Twitch Chat Command Cheat Sheet
Cheat sheet of chat command for stream elements, stream labs and nightbot. 

# Menu
* [Global things](#global-things)
* [Streamlabs](#streamlabs)
    * [Variables](#variables)
    * [Commands](#Commands)
    * [Examples](#Examples)
* [StreamElements](#streamElements)
    * [Variables](#variables-1)
    * [Commands](#Commands-1)
    * [Examples](#Examples-1)
* [Nightbot](#nightbot)
    * [Variables](#variables-2)
    * [Commands](#Commands-2)
    * [Examples](#Examples-2)

# Global Things
* ``` /me ``` - Adding this before the command text changes the text color to the bot's color
* ``` !settitle ``` - Set the title of the stream

# Streamlabs

## Variables
* ``` {target.name} ```
* ``` {user} ```
    * ``` {user.name} ```
    * ``` {user.time} ```
* ``` {touser} ``` - Adds an @ before the user's name
    * ``` {touser.name} ```
    * ``` {touser.followage} ``` Shows how long the user has been following the channel
* ``` {uptime} ``` - Shows how long the user has been currently streaming
* ``` {channel} ```
    * ``` {channel.name} ``` - Streamer's name
    * ``` {channel.followers} ``` - Current followers for the streamer
    * ``` {channel.subs} ``` - Current subs for the streamer
* ``` {randnum.minNumber-MaxNumber}``` - Outputs a random number between the range you give it, checkout examples to see how to use it

## Commands
* Add command
    * ```!addcommand !commandName Command will say this ```
* Edit command
    * ``` !editcommand !commandName Command will change to say this ```
* Remove command
    * ``` !removecommand !commandName ```

## Examples
* ``` !addcommand !hug {user.name} is giving {target.name} a big warm  hug. ```

* ``` !editcommand !uptime Dj tester has been streaming for {uptime}!!! ```
	
* ``` !removecommand !hug ```
	
* ``` !settitle Title of Stream :D ```

* ``` !addcommand !followers Dj Little Rock has {channel.followers}  followers! :pog: ```

* ``` !addcommand !followage {touser.name} has been following {channel. name} for {touser.followage} ```

* ``` !editcommand !subs DjNotes has {channel.subs} subscribers! <3 ```

* ``` !editcommand !uptime /me Dj tester has been streaming for {uptime} !!! ```

* ``` !addcommand !vibeTest {user.name} got a {randnum.0-100}% on their vibin test! ```


# StreamElements

## Variables
* ``` ${sender} ``` works like user in streamlabs
* ``` ${user} or ${1}  ```
* ``` ${touser}  ``` 
* ``` ${uptime} ```
* ``` ${channel} ```
    * ``` ${channel.followers} ``` - Current followers for the streamer
    * ``` ${channel.subscribers} ``` - Current subs for the streamer
    * ``` ${channel.alias} ``` - Streamer's name
* ``` ${random.minNumber-MaxNumber}``` - Outputs a random number between the range you give it
 
## Commands
* Add command
    * ```!command add !commandName Text for the command ```
* Edit command
    * ```!command edit !commandName Edited text ```
* Remove command
    * ```!command remove !commandName  ```

## Examples
* ```!command add !br {sender} or {user.name} is currently body rolling ```

* ```!command edit !hug {sender} is hugging {user} ```

* ```!command remove !so ```

* ```!command add !subs ${channel.alias} has ${channel.subscribers}!! ```

* ```!command add !so Checkout ${user} at www.twitch.tv/${user} ```

* ```!command edit !followers ${channel.alias} has ${channel.followers}!! ```

* ``` !command edit !so /me $(user) was last seen in "$(game $(user))" at twitch.tv/$(user) ! Go check them out, you King & Queens!~ ```

* ``` !command add !vibeTest ${user} is ${random.0-100}% vibin```

# NightBot
## Variables
    
## Commands
* Add command
    * ``` !commands add !commandName Text for the command```

* Edit command
    * ``` !commands edit !commandName CHange the previous command text ```

* Remove command
    * ``` !commands remove !commandName ```

# Examples

