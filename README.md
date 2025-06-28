# AzerothCore High Elf

Mod to add High Elves as playable characters on Azeroth Core with support for mod-playerbots.

By abracadaniel222.

## Goals

I am not familiar with modding so the goals for this project were very simple and limited, allowing for quick feedback and a quick POC:

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
- Hair clipping for some helmets for female High Elf
- Race change is untested (once I do, I might update this project)

## Other considerations

- AzerothCore supports modules but the race list is hardcoded and can't be extended, so this "module" consists of a patch to be applied to AzerothCore core code after cloning it. Another option would be forking and keeping it up-to-date with the source but maintaining that would go against the simplicity constraints of this project.

## Installation

Make sure you understand what each file and command does, and adjust the steps accordingly based on your setup. It is likely that some things don't apply to you if you don't have a Ubuntu + Playerbots setup.

Installation consists of applying a patch and replacing DBC files on the server, and applying some mpq patches on the client.

1. Fully install and configure Azeroth Core with or without playerbots. Installing and setting up the basic Azeroth Core is out of scope of this doc. Installation instructions can be found in https://www.azerothcore.org/ .
2. Follow the instructions in [Installation step by step.txt](./Installation step by step.txt).

## How this was built

With the help of the WoW Modding Community channel on Discord and https://github.com/araxiaonline/mod-worgoblin.

See DBC `Creation Step by Step.txt` and `DBC Creation Step by Step SQL.sql`.
