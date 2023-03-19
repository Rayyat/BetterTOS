# BetterTOS

BetterTOS is the first ever Town of Salem mod which adds new roles, QoL improvements and custom music to the game.

## How does this work ?
This mod DOES NOT change the base game. The mod adds 2 modded game modes, namely All Any+ and Custom to it, which is the place new content is in.

Vanilla game can be played when the mod is installed, but the new content will not be in the base game. However QoL changes will work for the base game as well.

It is recommended to use this mod with the Quality of Life mod, but it is not necessary.

## Manual Update Instructions

 BetterTOS has an auto updater feature that automatically updates the mod whenever an update is dropped. But in cases it doesn't work , you have to manually update the mod.

1. Download the DLL file only from the latest release
2. Find the folder of your game. You can right click on the game in your library, a menu will appear, click on properties, local data, browse
3. Navigate to BepInEx/plugins
4. Replace the DLL with the one you downloaded.
5. Run the game

## Windows Installation

1. Download the latest Windows ZIP from [the latest release](https://github.com/Rayyat/BetterTOS/releases) to install the mod
2. Find the folder of your game. You can right click on the game in your library, a menu will appear, click on properties, local data, browse
3. Now unzip and drag or extract the files from the .zip into your Town of Salem game folder that you just copied, at the .exe level (just into the folder).
4. Run the game from Steam (the first launch might take a while).

## macOS Installation (without Wine)

1. Download the latest Mac ZIP from [the latest release](https://github.com/Rayyat/BetterTOS/releases) to install the mod
2. Find the folder of your game. You can right click on the game in your library, a menu will appear, click on properties, local data, browse
3. Now unzip and drag or extract the files from the .zip into your Town of Salem game folder that you just copied, at the .app level (just into the folder).
4. Open the included run script "run_bepinex.sh" in a text editor of your choice. Edit the line executable_name=""; into executable_name="TownOfSalem.app";
5. Open the terminal in the game folder and run this command: 
```
chmod u+x run_bepinex.sh
```
6. Open the game's properties on Steam , then click "Set launch options" , and set it to
```
/bin/sh run_bepinex.sh %command%
```

7. Run the game from Steam (the first launch might take a while).


# Releases
| Town of Salem - Version| Mod Version | Link |
|----------|-------------|-----------------|
| v3.3.8 | v1.0 |N/A
| v3.3.8 | v1.1 | N/A
| v3.3.8 | v1.1.1 | [Download](https://github.com/Rayyat/BetterTOS/releases/tag/v1.1.1)

# New Roles
| Mafia | Town | Neutral |
|----------|-------------|-----------------|
| [Agent](#agent-mafia-support) | [Marshall](#marshall-town-support) | [Jackal](#jackal-neutral-chaos) |
| [Beguiler](#beguiler-mafia-deception) | [Handler](#handler-town-protective) | [Judge](#judge-neutral-evil)
| [Kidnapper](#kidnapper-mafia-killing) |   | [Auditor](#auditor-neutral-evil)

## Agent (Mafia Support)
This role can stalk someone at night and see who visits them. You have no limits unlike LO who can see maximum of 3 people.

Investigative Results: LO/Forger/Witch/Agent

Sheriff : Suspicious

## Beguiler (Mafia Deception)
You may hide a Mafia member including yourself at someone's house and redirect anyone who visits the Mafia member to your target. You may do this 3 times.

Investigative Results: Framer/Vampire/Jester/Beguiler

Sheriff : Suspicious

## Judge (Neutral Evil)
You may call court and force an anonymous vote where your votes count as 3 votes and whoever gets voted up instantly gets lynched. Votes are anonymous during court. This only lasts one day.
You may do this once.

Investigative Results: Invest/Consig/Mayor/Judge/Marshall

Sheriff : Innocent

## Auditor (Neutral Evil)
The Auditor is a Neutral Evil role that has two abilities: Smokebomb (prevent a player from learning what happens to them at night, along with preventing their visitors from getting notifications on their target) and Audit (roleblock a player and steal a charge from them, if any).

Investigative Results: Escort/Transporter/Consort/Hypnotist/Auditor

Sheriff : Innocent

## Jackal (Neutral Chaos)
You start the game with 2 recruits , one of them being Town/NE/Survivor, the other one being Mafia/NK. The recruits must win together with the Jackal regardless of their original faction. The recruits are lifelinked to each other , meaning if one of the recruits dies the other one will die as well. The Jackal won't die in that case though.
If the recruits die the Jackal gains a 1-time assassination, dealing a Powerful attack to one person.

Executioner,Jester,Amnesiac or BG cannot be a recruit.

This role is intended to replace the Lovers mechanic for the mod, instead of multiple couples there will be one couple aka Team Jackal if a Jackal spawns, but it will be much stronger.

Investigative Results: Sheriff/Exe/Ww/Jackal

Sheriff : Innocent

## Kidnapper (Mafia Killing)
You may kidnap someone during the day and optionally execute them once(starting from N2.) You may not kidnap a revealed Mayor. If you try to kidnap the Jailor or a jailed person, it will fail. If you kidnap someone and the Jailor jails you at the same time, your kidnap will fail and you will be jailed.

Investigative Results: Spy/BM/Jailor/Kidnapper

Sheriff : Suspicious

## Marshall (Town Support)
During the day you may reveal yourself to allow multiple lynches happen during the same day. You may do this once. Your votes count as 2 votes during the group lynch and revert back to 1 vote the next day. The Town will learn the lynched people's roles after the group lynch is over.

Investigative Results: Invest/Consig/Mayor/Judge/Marshall

Sheriff : Innocent

## Handler (Town Protective)
Handler is a Town role that can send a guard dog to protect someone at night. The hound will catch an attacker's scent if they scared off an attack. If you visit a player that you have the scent of, or you save someone from an attacker who you have the scent of, you will know who they are.

Investigative Results: Bodyguard/Godfather/Arsonist/Handler

Sheriff : Innocent

# Discord Rich Presence

Town of Salem is a game that lacks a Discord Rich Presence, but BetterTOS is here to fill that space up! BetterTOS mod adds a proper Discord Rich Presence with more info about the game you can show off!

Known Issue: Discord RPC only works in Windows right now. In future builds Mac and Linux will also support this feature.

<img src="/richpresence.png"/>


# Custom Options

## Ban/Unban Roles
Hosts can ban roles with these commands.

`/banrole <role name>`

`/unbanrole <role name>`

## Disable Names
Hosts can disable picking names in Custom lobbies.

`/disablenames`

`/enablenames`

## Disable Names
Hosts can enable modifiers in Custom lobbies.

`/tt`


#

# FAQ
## Where's the source code ?
The mod is closed-source due to people using modding in a malicious way, exploiting the base game. You can DNspy the code to see it for yourself , but I will not share the server code.
## Is this mod safe to use ?
Yes, people use DNspy on the code frequently and can confirm there is nothing bad. Alternatively, use the tool on my code before running it yourself if you want to be certain. BlankMediaGames aren't against this mod , so there is 0 risk of ban.
## Does this mod have Coven in it ?
No, not yet. It would be access to paid DLC roles with non-Coven accounts if it were a thing. You do not need the Coven DLC to use the mod.
## Can I play this mod on Web or Mobile versions ?
No. The mod authenticates players based on their Steam account. so it won't be possible for this mod to be played in Web. And there is no possible way to mod the game in Mobile. So the mod is only for Steam version of ToS.


# Bugs / Suggestions

If you found a bug and want to report it or you want to suggest something , join the [Discord Server](https://discord.gg/tubaantics) here!

#

This mod is not affiliated with Town of Salem or BlankMediaGames, and the content contained therein is not endorsed or otherwise sponsored by BlankMediaGames. Portions of the materials contained herein are property of BlankMediaGames.

© BlankMediaGames
