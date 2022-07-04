# IUV2-Docs
crying internally
discord.gg/callie / Basic#2142

# How to get your roli-token
```
> "roli_token"
1. Go to "https://www.rolimons.com/tradeadcreate"
2. Login to Rolimons (if you aren't already) and inspect the web page
3. Go to the network tab and refresh the page 
4. Click the first request called "tradeadcreate" and scroll down to the request headers section
5. Find cookie section of the header then copy the token after "_RoliVerification=" token until the "_RoliData" token starts 
6. Paste the token in the string that follows "roli_token": in the config.json file
```

# How to get a discordbot token (and make one)
```
> "bot_token"
1. Go to "https://discord.com/developers/applications" and login to your discord account
2. Press "New Application" and name the bot anything you'd like
3. Click the three bars at the top right of the screen and click the "Bot" tab (if you don't see the 3 dots just click the "bot" tab omfg)
4. Create a bot and click "reveal token"
5. Copy the token and paste it into the string that follows "bot_token": in the config.json file
6. Go back to the sub-menu that you got through step 3 and pess "OAuth2" then press "URL Generator"
7. Click the "Bot" check-mark under scopes and give the bot "Administrator" permisisons.
8. Copy the Generated link and use it to invite the bot to your server
```

# Documentation

```
:: Auth ::
  > cookie:
    Your Roblox cookie.
  > Key
    Your IU key.
:: trade_bot ::
  > run_file
    The .exe your tradebot uses to run, leaving this empty will let you run IU without a tradebot.
  > config_file
    The config file for your tradebot, you don't need to fill this in but config related commands will break.
:: discord_bot ::
  > token 
    Your discordbot token, see above for how to make a discordbot and get its token.
  > discordid
    Your discord ID (right click your profile).
  > bot_prefix 
    The prefix for your commands (ex: !help, "!" would be the prefix).
  > Channels
    The channels you'd like the bot to notify tradeads, completeds, outbounds, and inbounds.
  > Mention
    The @ (discord mention) you'd like the bot to use:
    Specific user format - <@DISCORDID>
    Specific role format - <@&ROLEID>
:: completeds ::
  > ?
    Whether it'll notify completeds or not.
  > check_int
    The delay between completed checks.
:: trade-ads :: 
  > roli-token
    Your rolimons token, see above if you need to know how to get it.
  > type
    The type of ads you'd like it to post, 
    restate: reposts your outbounds as trade ads
    top: posts your top items as an ad
:: inbounds ::
  > notify?
    Whether or not it'll notify your inbounds.
  > send_wins_only
    Wether or not you'd like IU to only notify good inbounds (according to your config/valuing).
  > cache_int 
    The delay between the times IU gets new inbounds.
:: outbounds :: 
  > check? 
    Whether or not you'd like IU to check your outbounds.
  > cache_int
   The delay between the times IU gets new outbounds.
:: valuing ::
  > ATB
    Whether or not you'd like IU to use an ATB config to value your inbounds/outbounds
  > ratios
    The ratios for mixed (same amt of items on each side), downgrade (more items on the requesting side), upgrade (less items on the requesting side) trades.
  > offer_values
    Additions to existing Rolimons values on the offer side ("id": "amount you'd like to add to the item's value w/ +/-").
  > request_values
    Additions to existing Rolimons values on the request side ("id": "amount you'd like to add to the item's value w/ +/-").
  > Projecteds
    The ratios for owned and requesting projecteds (if you don't want projecteds set "requesting_ratio" to 0.
:: auto_config ::
  > ?
    Wether you'd like IU to automatically configure ATB v2.03's config (on completeds as well).
  > keep_base
    Keeps your base config (ratios) when configuring it.
  > auto_type
    IU will automatically decide whether your bot will send upgrades, downgrades, and mixed trades based on the amount of items you have.
  > configure_projs
    Allows IU to set ratios which lowball your projecteds by a certain amount.
```
