# Steamlaunchy

A tiny wrapper to programmatically launch third-party windows applications from within Steam

## Usage

```
steamlaunchy <path/to/exe>
```

## Environment Variables

```
STEAMLAUNCHY_CONF                  Override Steamlaunchy config. A config file is optional
STEAMLAUNCHY_DEBUG                 Set to '1' to increase logging
STEAMLAUNCHY_STEAM_HOME            Override default Steam installation dir
STEAMLAUNCHY_PROTON_PATH           Override Proton versions available to Steamlaunchy. By default it searches the Steam installation dir. Comma delimited string of proton dir paths
STEAMLAUNCHY_PROTON_VERSION        Override default Proton version. By default the lastest stable Proton version is selected
STEAMLAUNCHY_PROTON_BIN            Override absolute path to Proton executable
STEAMLAUNCHY_PROTON_BIN_NAME       Override Proton executable basename
STEAMLAUNCHY_INCLUDE_EXPERIMENTAL  Set to `1` to include non-semantic Proton versions in Proton version selection
```
