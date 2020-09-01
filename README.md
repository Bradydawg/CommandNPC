![CommandNPC](https://i.imgur.com/awdxHuc.png)

##CommandNPC
CommandNPC is a plugin inspired by the server Mineplex, which adds a new function to NPCs. It allows users to run commands by simply right clicking on a Citizens NPC. Requires Citizens 2! Keep in mind, if you are an early adopter for any update. If it says unknown webpage, please wait until the BukkitDev staff approve the plugin first. Once approved you'll be able to see it. REQUIRES JAVA 8!

**Command NPC Latest Version - ![https://github.com/Bradydawg/CommandNPC/releases/tag/2.0](https://img.shields.io/github/v/release/Bradydawg/CommandNPC)**

##Discord
[![Discord](https://i.imgur.com/UxvvtYw.png)](https://discord.gg/BpNs7DA)

##Commands and Permissions

(Now supports PlaceholderAPI)

To set up the npc with the commands you need the permission 'commandnpc.admin'
Be aware that flags that require additional input like [--v price], you need 2 dashes(-)!

/npc cmdadd [-c console] [-o Op] [-r random] [-i ignorePermMsg] [-l ignoreMoneyMsg] [--v price] [--t clickType] [--d delay] [--cd cooldown] [--p custom.permission.node] <command...> - Add a command to be executed upon clicking the selected NPC.
- The -c flag runs the command through the console.
- The -o flag runs the command as an op.
- The -r flag picks a random command and executes that one command only.
- The -i flag when true, noPerm message doesn't send
- The -l flag when true, noMoney message doesn't send
- The --v flag charges the player the specified amount, when running the command. (Numeric with decimal)
- The --p flag requires the player to have the specified permission.
- The --d flag is the amount of ticks that the command will be delayed by. (Integer input)
- The --cd flag is a cooldown for the command in ticks. (20 ticks in a second)
- The --t flag sets the clickType('left', 'right', or 'both') | This will default to the global setting in config.yml

/npc cmdinfo [id] - Gets various information about all the NPC commands
- If you include the command 'id' it will only show information for that command.
- You get the 'id' from using the 'cmdinfo' command

/npc cmdremove <id> - Removes a specific command
- You get the 'id' from using the 'cmdinfo' command

/npc cmdset [-c console] [-o Op] [-r random] [-m cdMsg] [-i ignorePermMsg] [-l ignoreMoneyMsg] [--v price] [--t clickType] [--d delay] [--cd cooldown] [--p custom.permission.node] [command | cdMsg...]- Set various variables for the command
- The -c flag runs the command through the console. (This will toggle between true/false)
- The -o flag runs the command as an op. (This will toggle between true/false)
- The -r flag picks a random command and executes that one command only.
- The -m flag is when you have a cooldown amount specified. When the player is in a cooldown and attempt to use the NPC, it will send them this message. (Usage: /npc cmdset -m [cdMsg...]) Note: When using other flags the cdMsg as to be the last things within the command.
- The -i flag when true, noPerm message doesn't send
- The -l flag when true, noMoney message doesn't send
- The --v flag charges the player the specified amount, when running the command. (Numeric with decimal)
- The --p flag requires the player to have the specified permission.
- The --d flag is the amount of ticks that the command will be delayed by. (Integer input)
- The --cd flag is a cooldown for the command in ticks. (20 ticks in a second)
- The --t flag sets the clickType ('left', 'right', or 'both')
- You get the 'id' from using the 'cmdinfo' command

/npc cmdreset - Remove all commands from the selected NPC.
- You can use '%name' in commands as a placeholder for the user who is clicking the NPC.
- This plugin now supports a BungeeCord command. You may now use 'server <serverName>' to teleport people between servers!

**How to setup the NPC**
1. Edit config.yml to your likings
2. Select the NPC you wish to add commands too.
3. Use the command 'cmdadd' (Syntax listed above) to add the commands you wish.
4. These commands will be saved.
5. If you wish to remove the commands simply use the 'resetcmds' command. (Syntax listed above)

**Metrics by bStats**
https://bstats.org/plugin/bukkit/CommandNPC

**Github**
https://github.com/Bradydawg/CommandNPC