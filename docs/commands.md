---
hide:
  - navigation
  - toc
---

# Commands

Here is a list of all the commands implemented by Solstice, along the permission node and aliases.

!!! note

    - Arguments surrounded by angle brackets (`<arg>`) are mandatory to supply.
    - Arguments surrounded by square brackets (`[arg]`) are optional.


| Command                                                                  | Permission node                    | Description                                                                             | Aliases              |
| ------------------------------------------------------------------------ | ---------------------------------- | --------------------------------------------------------------------------------------- | -------------------- |
| `/broadcast <message>`                                                   | `solstice.command.broadcast`       | Broadcast a message to all players.                                                     |                      |
| `/restart schedule <seconds [message], next>`                            | `solstice.command.restart`         | Start a countdown to server restart. `next` schedules for the next configured restart.  |                      |
| `/restart cancel`                                                        | `solstice.command.restart`         | Cancel the scheduled restart.                                                           |                      |
| `/solstice`                                                              | `solstice.command.solstice`        | Display version of the mod.                                                             |                      |
| `/solstice reload`                                                       | `solstice.command.solstice.reload` | Reload the mod configuration, useful for changes without needing to restart.            |                      |
| `/sudo <command>`                                                        | `solstice.command.sudo`            | Run a command as server.                                                                |                      |
| `/doas <player> <command>`                                               | `solstice.command.doas`            | Run a command as player.                                                                |                      |
| `/timebar start <seconds> <color> <style> <countdown> <label> <command>` | `solstice.command.timebar`         | Start boss bar that progresses (or counts down) and then run a command as the executer. |                      |
| `/timebar cancel <uuid>`                                                 | `solstice.command.timerbar`        | Cancel a timebar.                                                                       |                      |
| `/feed <players>`                                                        | `solstice.command.feed`            | Feed players to their max hunger and saturation.                                        |                      |
| `/heal <entities>`                                                       | `solstice.command.heal`            | Heal entities to their max health.                                                      |                      |
| `/fly [player]`                                                          | `solstice.command.fly`             | Toggle creative flight.                                                                 |                      |
| `/god [player]`                                                          | `solstice.command.god`             | Toggle invulnerability.                                                                 |                      |
| `/nick <nickname>`                                                       | `solstice.command.nick`            | Set your nickname.                                                                      |                      |
| `/nick clear`                                                            | `solstice.command.nick`            | Clear your nickname.                                                                    |                      |
| `/nick <player> <nickname>`                                              | `solstice.command.nick`            | Set a player nickname.                                                                  |                      |
| `/nick <player> clear`                                                   | `solstice.command.nick`            | Clear a player nickname.                                                                |                      |
| `/smite <target> [times]`                                                | `solstice.command.smite`           | Summon a lightning bolt on a target.                                                    |                      |
| `/home [home]`                                                           | `solstice.command.home`            | Teleport to a home.                                                                     |                      |
| `/sethome [home] [force]`                                                | `solstice.command.sethome`         | Set a home. Will prompt if already existing.                                            |                      |
| `/delhome [home]`                                                        | `solstice.command.delhome`         | Delete a home.                                                                          |                      |
| `/homes`                                                                 | `solstice.command.homes`           | List all homes.                                                                         |                      |
| `/afk`                                                                   | `solstice.command.afk`             | Go away from keyboard.                                                                  |                      |
| `/info [page]`                                                           | `solstice.command.info`            | Read an info page.                                                                      |                      |
| `/mail`                                                                  | `solstice.command.mail`            | List all mails in the inbox.                                                            |                      |
| `/mail send <recipient> <message>`                                       | `solstice.command.mail`            | Send a mail to a player.                                                                |                      |
| `/mail read <index>`                                                     | `solstice.command.mail`            | Read a mail from the inbox.                                                             |                      |
| `/mail delete <index>`                                                   | `solstice.command.mail`            | Delete a mail from the inbox.                                                           |                      |
| `/motd`                                                                  | `solstice.command.motd`            | Show the message of the day. This is an info page.                                      |                      |
| `/near [range]`                                                          | `solstice.command.near`            | Get all players in the range.                                                           |                      |
| `/rules`                                                                 | `soltice.command.rules`            | Show the rules info page.                                                               |                      |
| `/seen`                                                                  | `soltice.command.seen`             | See first login and last logout of a player.                                            |                      |
| `/seen` (extended)                                                       | `solstice.command.seen.extended`   | Extends base `/seen` to display IP address and location in the server.                  |                      |
| `/suicide`                                                               | `solstice.command.suicide`         | Insta-kill your player.                                                                 |                      |
| `/ban <targets> [reason]`                                                | `solstice.command.ban`             | Permanently ban players.                                                                |                      |
| `/tempban <targets> <duration> [reason]`                                 | `solstice.command.tempban`         | Temporary ban players.                                                                  |                      |
| `/unban <targets>`                                                       | `solstice.command.unban`           | Pardon and unban players.                                                               | `/pardon`            |
| `/kick <targets> [message]`                                              | `solstice.command.kick`            | Kick players out of the server.                                                         |                      |
| `/mute <players>`                                                        | `solstice.command.mute`            | Mute players, they will not be able to chat.                                            |                      |
| `/ignore <players>`                                                      | `solstice.command.ignore`          | Ignore a player. All their messages, DMs, TPAs, mails will be silently ignored.         |                      |
| `/ignorelist`                                                            | `solstice.command.ignorelist`      | Get a list of ignored players.                                                          |                      |
| `/spawn`                                                                 | `solstice.command.spawn`           | Teleport to the server spawn.                                                           |                      |
| `/spawn <players>`                                                       | `solstice.command.spawn.other`     | Teleport players to spawn.                                                              |                      |
| `/setspawn`                                                              | `solstice.command.setspawn`        | Set the server spawn. This command also sets the world spawn.                           |                      |
| `/delspawn`                                                              | `solstice.command.delspawn`        | Delete the server spawn. This will not delete the world spawn.                          |                      |
| `/back`                                                                  | `solstice.command.back`            | Teleport to the previous position before teleport.                                      |                      |
| `/tpaccept [uuid]`                                                       | `solstice.command.tpaccept`        | Accept a teleport request.                                                              | `/tpyes`             |
| `/tpdeny [uuid]`                                                         | `solstice.command.tpdeny`          | Refuse a teleport request.                                                              | `/tpno`, `/tprefuse` |
| `/tpa <player>`                                                          | `solstice.command.tpa`             | Request to teleport to a player.                                                        | `/tpask`             |
| `/tpahere <player>`                                                      | `solstice.command.tpahere`         | Request a player to teleport to you.                                                    | `/tpaskhere`         |
| `/tphere <targets>`                                                      | `solstice.command.tphere`          | Teleport targets to you.                                                                |                      |
| `/tpoffline <player>`                                                    | `solstice.command.tpoffline`       | Teleport to an offline player's last location.                                          |                      |
| `/tell <player> <message>`                                               | `solstice.command.tell`            | Send a direct message to a player.                                                      | `/msg`, `/w`, `/dm`  |
| `/tell Server <message>`                                                 | `solstice.command.tell`            | Send a direct message to the server.                                                    | `/msg`, `/w`, `/dm`  |
| `/reply <message>`                                                       | `solstice.command.reply`           | Reply to the latest direct message.                                                     | `/r`                 |
| `/warps`                                                                 | `solstice.command.warps`           | Shows a list of all the available warp waypoints.                                       |                      |
| `/warp <name>`                                                           | `solstice.command.warp`            | Teleport to a warp waypoint.                                                            |                      |
| `/setwarp <name>`                                                        | `solstice.command.setwarp`         | Delete a warp waypoint.                                                                 |                      |
| `/delwarp <name>`                                                        | `solstice.command.delwarp`         | Set a warp waypoint.                                                                    |                      |