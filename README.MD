# Honeygold
**_An easy-on-the-eyes dark theme with gold highlights for qBittorrent_**

### Supported qBittorrent versions
- Working on 4.3.1--4.4.5
- Does not work in 4.5 and after (will be supported when qBt devs fix WebUI translation)

[Small preview](screens/1.png)
[Larger preview](screens/2.png)

# Feature set
1. Honeygold has a 'Linux ISO mode' which redact your torrent names and replaces them with Linux ISO names (bottom right corner - the eye icon)
2. 'Last Activity' column functions normally (compared to Nightwalker)
3. The auxiliary windows are properly rendered (compared to Nightwalker)
4. Has nice ratio highlights:
- ![#8f8f8f](https://placehold.co/15x15/8f8f8f/8f8f8f.png) `< 1`
- ![#ffffff](https://placehold.co/15x15/ffffff/ffffff.png) `< 2`
- ![#1eff00](https://placehold.co/15x15/1eff00/1eff00.png) `< 10`
- ![#0070dd](https://placehold.co/15x15/0070dd/0070dd.png) `< 20`
- ![#a335ee](https://placehold.co/15x15/a335ee/a335ee.png) `< 60`
- ![#ff8000](https://placehold.co/15x15/ff8000/ff8000.png) `< 90`
- ![#e6cc80](https://placehold.co/15x15/e6cc80/e6cc80.png) `< 100`
- ? `> 100` (secret)


# Installation

### Linux
1. `sudo -i`
2. `mkdir -p && cd /opt`
3. `git clone https://github.com/stacksmash76/qbt-honeygold.git honeygold`
4. `chown -R nobody:nogroup honeygold`


### Activate Alterative WebUI in qBittorrent
1. Under `Tools->Preferences->WebUI` enable `Use alternative WebUI`.
2. Choose a location that points to the `honeygold` folder, i.e. `/opt/honeygold/`
3. Restart qBittorrent or refresh your browser for changes to take effect.


You can also change these settings via the config file, which is usually located at `~/.config/qBittorrent/qBittorrent.conf`. The relevant entries are:

- `WebUI\AlternativeUIEnabled=true`
- `WebUI\RootFolder=/opt/honeygold/`

(If something breaks for any reason whatsoever, you can also use this method to revert any bad changes if the WebUI is unresponsive)


### Update theme (Linux)
1. `cd /opt/honeywell`
2. `sudo git pull`


# Credits
- qBittorrent devs
- repslet and imabee (for Nightwalker)
- gl0ryus
- Iconmonstr (icons)
- FontAwesome (icons)
- Radix (colors)
