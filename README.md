# RAID Toolkit

***RAID Toolkit*** is a companion application designed to be run alongside *RAID: Shadow Legends* and will provide additional features and aids to players.
***This is NOT built as a cheating application, and will never entertain providing capabilities which could not be accomplished without the tool.***

[Download latest release](http://raid-bot.eastus.azurecontainer.io/hazel)

## Current features

### Mercy Shard Status
Tired of keeping a spreadsheet/notebook and logging all of your pulls so you know when you're due for a Mercy Rule legendary? This tab will show you the number of pulls of each shard type you've had since you pulled a given rarity, as well as your current summoning chances for that shard/rarity combination and most recent pull.

![image](https://user-images.githubusercontent.com/500984/115713732-57bc6480-a344-11eb-802b-0af2f052bb0c.png)

### Heroes Roster
View all the heroes in your account in one place, with sorting and filtering (including dungeon team filters!).

![image](https://user-images.githubusercontent.com/500984/115713910-89cdc680-a344-11eb-9f14-1d14bfdbb0be.png)

#### Damage Calculator
The hero details view will also attempt to estimate the damage of each champions skill based on their stats, books, masteries, and some optional flags you can tweak. 

![image](https://user-images.githubusercontent.com/500984/115714011-a833c200-a344-11eb-961e-142333481f36.png)

> The damage calculator is still in progress, so some of the values will be off.  If you find one that is obviously calculated incorrectly, please log an issue here and I'll try to fix it as soon as I can.


### Account Data Export
You can enable a local `rest` endpoint from the tool which will allow you to import your data into Excel or even other future applications which are built to use this tool. Simply click export icon in the top right of the application, and then you can point your favorite tool at the endpoint it lists (`localhost:5656/champions`). This endpoint will dump all of your champion data in one (giant) JSON object. You can import this data into Excel, or any other tool. You can even build your own tool to use this data.

![image](https://user-images.githubusercontent.com/500984/115713836-728ed900-a344-11eb-9fb5-a4d4a55d070e.png)


# FAQ

## Why is this tool not open source?
Because of *how* this application is designed and coded, there's enough risk that others could use its code for malicious purposes (such as cheating) in the game, and that is not something I want to facilitate. While these things could be done without this applications code, it requires a decent amount of work and internal knowledge of how the Unity Engine and il2cpp works to accomplish.

I do plan to release the libraries I've created for code generation using il2js metadata at a later date once I can generalize them further than they are today.
