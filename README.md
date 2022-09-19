# Steamlaunchy

A tiny wrapper to programmatically launch third-party windows applications from within Steam

## Usage

```
steamlaunchy <path/to/exe>
```

### Advanced

1. Overriding Application Prefix

By default each executable is assigned a random prefix (`~/.local/share/steamlaunchy/<randomInteger>`). You may override the prefix name with variable `STEAMLAUNCHY_APPLICATION_PREFIX`

```
STEAMLAUNCHY_APPLICATION_PREFIX=FooBar steamlaunchy </path/to/exe>
```

This will create directory `~/.local/share/steamlaunchy/FooBar`

## Environment Variables

```
STEAMLAUNCHY_CONFIG_HOME           Defaults to '~/.config/steamlaunchy'
STEAMLAUNCHY_DATA_HOME             Defaults to '~/.local/share/steamlaunchy'
STEAMLAUNCHY_CONF                  Override Steamlaunchy config. A config file is optional
STEAMLAUNCHY_DEBUG                 Set to '1' to increase logging
STEAMLAUNCHY_PROTON_PATH           Override Proton versions available to Steamlaunchy. By default it searches the Steam installation dir. Comma delimited string of proton dir paths
STEAMLAUNCHY_PROTON_VERSION        Override default Proton version. By default the lastest stable Proton version is selected
STEAMLAUNCHY_PROTON_BIN            Override absolute path to Proton executable
STEAMLAUNCHY_PROTON_BIN_NAME       Override Proton executable basename
STEAMLAUNCHY_INCLUDE_EXPERIMENTAL  Set to `1` to include non-semantic Proton versions in Proton version selection
STEAMLAUNCHY_APPLICATION_PREFIX    Override the application prefix in STEAMLAUNCHY_DATA_HOME
```

## Install

```
curl --proto '=https' --tlsv1.2 -sSf -o ~/.local/bin/steamlaunchy https://raw.githubusercontent.com/egladman/steamlaunchy/main/steamlaunchy
chmod +x ~/.local/bin/steamlaunchy
```
