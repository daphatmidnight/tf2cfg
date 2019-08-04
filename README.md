# unitgon's TF2 configs

Settings for a beefy desktop. Settings for someone who likes to use a fuckton of buttons on the keeb and mouse. Settings for unitgon. Because why not.

## Dependancies

* First-person shooty game "Team Fortress 2" by the Valve Corporation
* [mastercomfig performance configs](https://github.com/mastercoms/mastercomfig) v6.11.2+
  just chuck the following files into `tf/custom/`:
  * `mastercomfig-xxxxx-preset.vpk`
  * `mastercomfig-no-tutorial-addon.vpk`
  * `mastercomfig-mouse-tweaks-addon.vpk`
* **Linux only**: `gamemode`, `lib32-gamemode`, `cpupower` and `irqbalance`
* (Highly recommended) A custom HUD such as [yayahud](https://github.com/Yttrium-tYcLief/yayahud)
* `git` of course

## Instructions

### Setup
Make a folder with any name in your `tf/custom/` directory (such as `my_scripts`).

Clone this repository into that folder, and it **MUST** have the name `cfg`.

```sh
# Clone with HTTPS
git clone https://github.com/unitgon/tf2cfg.git cfg
# Clone with SSH
git clone git@github.com:unitgon/tf2cfg.git cfg
```

### Binds
Now you **MUST** make a `kbd.cfg` file. It executes `dvorak` or `qwerty`: it depends on your operating system for key detection in TF2.

```js
// Uncomment one of the following lines

// exec dvorak // For Windows if you use dvorak
// exec qwerty // Probably all other cases
```

### Launch Options
**Windows**:
```
-novid -softparticlesdefaultoff -reuse -nohltv -console -nostartupsound
```

**Linux**: (note: have you `systemctl --user enable`d and `start`ed the `gamemode` service?)
```
gamemoderun %command% -novid -softparticlesdefaultoff -reuse -nohltv -console -nostartupsound -NoQueuedPacketThread -freq 165 -gl_enablesamplerobjects -gl_texclientstorage
```

## Disclaimer
unitgon is not associated with Valve Corporation or Steam.

i made this for myself so i don't take responsibility for any major frick-ups you do on your part if you choose to use this

however i am open for a nice conversation, find me on steam or discord!
