## Testing Lisk Quick start

Lisk QuickStart: https://lisk.com/documentation/lisk-sdk/quickstart.html

Lisk does not seem to run in Windows, so running from

* WSL2 hosting Ubuntu 20.04
* Node v12

```bash
# Install node
nvm install 12.22.1
nvm use 12.22.1
node -v
# v12.22.1

# Install Lisk CLI
npm install --global --production lisk-commander

# Create root folder
mkdir lsk-qstart1&&cd lsk-qstart1
# Scaffold project
lisk init
# Enter various data
```

When project is created you can see what it can do

```bash
# View App CLI commands
node ./bin/run
# See options for starting
node ./bin/run start -h
# Start a fresh blockchain node with a fresh genesis block
node ./bin/run start
# Ctrl-c to stop
```

# --- Org README -------------------
## Getting Started with Lisk Blockchain Client

This project was bootstrapped with [Lisk SDK](https://github.com/LiskHQ/lisk-sdk)

### Start a node
```
./bin/run start
```

### Add a new module
```
lisk generate:module ModuleName ModuleID
// Example
lisk generate:module token 1
```

### Add a new asset
```
lisk generate:asset ModuleName AssetName AssetID
// Example
lisk generate:asset token transfer 1
```

### Add a new plugin
```
lisk generate:plugin PluginAlias
// Example
lisk generate:plugin httpAPI
```

## Learn More

You can learn more in the [documentation](https://lisk.io/documentation/lisk-sdk/index.html).
