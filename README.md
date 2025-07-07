# AzerothCore High Elf

Mod to add High Elves as playable characters on Azeroth Core with support for mod-playerbots.

## Goals

The goals for this project are very simple and limited, allowing for quick feedback and a quick POC:

1. Duplicate blood elf models into a new high elf race
2. Copy everything else from humans (starting zone, mounts, reputation, quests, etc)

## Features

- A new High Elf alliance race is added
  - It shares the same models as the Blood Elf race
  - It shares the same starting zone, reputation, skills as the humans
  - High Elves can be any class except shaman or druid
- Compatible with HD models 

## Known limitations

- Eyes don't glow blue
- Warriors don't have Arcane Torrent
- No audio in emotes (such as /hi, /joke, etc)
- If High Elves start with no weapons skills, ensure that you don't have any modules modifying skills as it may conflict. Compatibility enhancements to this mod are welcomed!

## Open issues

- See [the issues page](https://github.com/abracadaniel22/azerothcore-highelf/issues) for known issues. Feel free to report anything there, or to fix issues if you are willing to contribute.

## Other considerations

- AzerothCore supports modules but the race list is hardcoded and can't be extended, so this "module" consists of a patch to be applied to AzerothCore core code after cloning it. Another option would be forking and keeping it up-to-date with the source but maintaining that would go against the simplicity constraints of this project.

## Requirements

- This requires a patched version of WoW.exe that allows interface edits (SIG & MD5 Protection removed). The version downloaded from Warmane or ChromieCraft should work. You can also download a patcher tool from the WoW Modding Community discord or from ownedcore.com and do it yourself. Without a patched version, the client will not accept the interface changes and will not allow you to play the game, throwing out errors such as "Your login interface files are corrupt".

## Installation

Make sure you understand what each file and command does, and adjust the steps accordingly based on your setup. It is likely that some things don't apply to you if you don't have a Ubuntu + Playerbots setup.

Installation consists of applying a patch and replacing DBC files on the server, and applying some mpq patches on the client.

1. Fully install and configure Azeroth Core with or without playerbots. Installing and setting up the basic Azeroth Core is out of scope of this doc. Installation instructions can be found in https://www.azerothcore.org/ .
2. Follow the instructions in `Installation step by step.txt`.

## How this was built

With the help of the WoW Modding Community channel on Discord and https://github.com/araxiaonline/mod-worgoblin.

See DBC `Creation Step by Step.txt` and `DBC Creation Step by Step SQL.sql`.

## Screenshots

![ss01](https://github.com/user-attachments/assets/55101550-e397-4f3e-91d1-ae6e60bd1f49)

![ss02](https://github.com/user-attachments/assets/d7f019c9-1169-4de4-bc34-2155a7582a83)

![ss03](https://github.com/user-attachments/assets/cf9944b4-17e0-4557-8d1b-086bfc18041f)
