# OpenFuji

This repository contains the software that runs the DrFujiBot Twitch chat bot. This chat bot provides Pokemon information, such as stats, moves, learn sets, evolution, type matchups, and more. The bot also supports custom commands, and various other silly features. It can also be run as a Discord bot. The bot is written in Python, and is meant to be run from a Linux server. All Pokemon information is pulled from a local PokeAPI instance.

The code was started as a simple, fun project, and grew over time as more ideas were added. Because of this approach, no planning or design was put into the initial code. As such, the code grew messy and harder to read. If you plan to work on the project, keep that thought in mind.

To view the re-write of this bot (which is a work in progress), look up MrFujiBot. MrFujiBot is a client-focused Windows application, written in C# and meant to be run locally by a streamer on their computer. Ideally, it will provide all the same features as DrFujiBot.

Despite plans for a re-write, OpenFuji is still in use by dozens of Twitch streamers, and continues to be maintained and improved. The OpenFuji instances running under the DrFujiBot Twitch account are hosted by everoddish.com

Several specific configuration values are missing from this repository (such as API keys, etc.) so that the DrFujiBot Twitch account remains protected. If you supply your own values for your own Twitch account, you may run the bot locally on your machine.

## Developing

1. Install dependencies

```
pip install -r requirements.txt
```

2. Create a streamer config (use SampleStreamer.json as a template)

3. Create the necessary meta files (these can be empty, but .json files must be valid JSON)
- PCCE.json
- bee.txt
- shaq.txt
- whisper_users.json

4. Fill in `DrFujiBot_config.json` with you bot user's info

5. Run the bot

```
bash drfujibot_launcher.sh my_config.json
```


