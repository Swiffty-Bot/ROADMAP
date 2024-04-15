# ROADMAP


### [Plugin Package](https://github.com/Swiffty-Bot/Plugin-Builder)
Package to create plugins with commands and events
- [X] Usage Docs
- [X] Create new plugin
- [X] Added name & description feilds
- [X] Ability to add command
- [X] Ability to add events
- [ ] Ability to bulk add commands from a folder
- [ ] Ability to bulk add events from folder
- [ ] Enable/Disable certain comands/events
- [ ] Events required for command to work
- [ ] Help command function to add commands to global help command
- [ ] Publish to Swiffty Plugins registry



### [Base Bot Structure](https://github.com/Swiffty-Bot/Base-Bot)
The structure of the base bot that will have customisable optiosn for the token and plugins dir path. The bot will also load events and commands as wel las regestering the commands. Bot includes basic function to run commands and events from the plugins.
- [X] Class extend of [discord.js client](https://discord.js.org/docs/packages/discord.js/14.14.1/Client:Class) with tokeen and plugin inputs
- [X] Start function to make the bot login
- [X] Load plugins from array store in plugin file
- [X] Register events from plugins and bind them to the client events
- [X] Load commands from plugins
- [X] Register commands with discord API
- [X] Proceess interaction event to run commands execute
- [ ] Detect if bot has reached limit of allowed slash commands
- [ ] Select custom intents
- [ ] Enable/Disable certain comands/events
- [ ] Events required for command to work
- [ ] Checks for conflicting command args


### [Swiffty Dashboard](https://github.com/Swiffty-Bot/Swiffty-Dashboard)
Dashboard to build & customise your bot. Create new bots, view bots stats, edit bots settings..including intents, plugins & more. Built with Tauri & React.
#### Backend
- [X] Initiallise tauri app
- [ ] Login with discord
- [ ] Routes to accept forms (possibly may be able to do this in frontend with react)
- [ ] Create base client with settings (token) & save to device in app config
- [ ] Fetch bot info
- [ ] Change enabled/disabled plugins stored in the local app config
- [ ] Install plugins from the registry to the local app config
- [ ] Install custom plugins from github repo/other sources
- [ ] Change bot intents stored in the main index.ts file of the bot
- [ ] Send console logs & info to frontend "termianl"
- [ ] Reveiwer page to review plugin requests to the registart
- [ ] Accept/deny plugin system see more at [plugin registry](https://github.com/Swiffty-Bot/Plugin-Registry)
#### Frontend
- [ ] Enitial landing page
- [ ] Dashboard page (display stats about the bot, name, profile pic, intents, enabled plugins)
- [ ] Plugins page (display all avaliable plugins from the registry)
- [ ] Plugin specific page (display all info about a plugin...name, creation data, author, description, git repo, required events, all commands)
- [ ] Import custom plugin pop down


### [Plugin Registry](https://github.com/Swiffty-Bot/Plugin-Registry)
Registry for all the public plugins.
- [ ] Connect to database server (not decided yet)
- [ ] Simple api with express (may change this to use a rust framework not sure)
- [ ] Route to submit a publish request (inputs: name, description, github repo)
- [ ] Route to submit a publish (requires reviewer token or something idk)
- [ ] Route to delete a plugin (requires author token)
- [ ] Route to get all info about a plugin
- [ ] Ratelimiter
