> **Note: It's "open-source" but thats doesn't mean that you can copy n paste and "steal" it! Thanks. Add me on discord or DM me on IG if you have any questions.**

<img align="right" src="http://gdszeged.hu/sites/default/files/storage/logo_gd.png" height="196" width="196">

# GD Discord BOT

A simple bot **GD BOT** which just tags you and notifies you on Discord in a specific channel.
Tags you or your group who has lesson.

# Idea

A user has the class and the group role, and if his class is present he or his group gets a ping in the server.
Everybody can add their own timetable (1file and has the groups n stuff).
The BOT can DM you and can notify you that your class is starting, also pings the server, it can be changed and managed in the future.

## How it works?

In a .js file we have the whole timetable. (Now just for my class 12E but we plan it to add others)
In a config.js we have the BOT and the token for it.
Hosted on heroku with a simple worker.

# Commands

> Note: Prefix is: /

|   Command    | Description                                 | Implementation | Command Syntax               | Response                      |
| :----------: | ------------------------------------------- | :------------: | ---------------------------- | ----------------------------- |
|     help     | Shows help                                  |       ✅       | help <'command'>             | Embed with summary.           |
|     info     | Shows full server info/summary.             |       ✅       | info                         | Shows server info.            |
|  clearchat   | clearing messages                           |       ✅       | clearchat or clearchat <'n'> | N/A                           |
|    reload    | reload a command                            |       ✅       | reload <'command'>           | Command reloaded.             |
|     ping     | Dev Command                                 |       ✅       | ping                         | BOT: Pong!                    |
|    getOra    | Get a specific class                        |       ❓       | getora <'lesson'>            | <'lesson'> will start at 8:00 |
| getTimeTable | Get the full timetable of a class           |       ❓       | getTimeTable <'12E:ID'>      | {timetable}                   |
|  checkClass  | Checks if a class is present                |       ❓       | checkClass <'12E:ID'>        | Yes, <'lesson'> óra van.      |
|     join     | Join to the User's active channel           |       ❌       | join or join <'channel'>     | N/A                           |
|     play     | Plays the added link                        |       ❌       | play <'link'>                | Track added to queue.         |
|    queue     | Show the full queue                         |       ❌       | queue                        | Shows the actual queue.       |
|     skip     | Skips the current track and plays instantly |       ❌       | skip or skip <'n'>           | Skipped <'n'> track.          |
|     loop     | Loops the current track/album               |       ❌       | loop <'queue ID'>            | Loop is enabled/disabled.     |
|     stop     | Stops the current track                     |       ❌       | stop                         | N/A                           |
|    leave     | Stops n leaves the channel                  |       ❌       | leave                        | N/A                           |

## Collaborate

1. Clone the repo
2. Enter a CLI and type `yarn install or npm i`
3. To start the development server type `npm run devStart`
4. Make changes
5. Open a PR (Pulll-Request)
6. Wait :)

# TODO

1. ✅ Make the bot parse the time and date, based on the lesson
2. ✅ Add command to get the timetable
3. ✅ Add command to get the current lesson
4. ✅ Add API
5. ❓ Collaborative something to upload 10 class and just import the one you need to work with it

> **Note:** It's still in development
