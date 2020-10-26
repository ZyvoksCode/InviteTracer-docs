# Full Config Reference

## Configs

There are many config options that can be set. You don't have to set all of them. If you just added the bot, just run `!setup`, which will guide you through the most important ones.

## Basic

* [prefix](configs.md#prefix)
* [lang](configs.md#lang)
* [logChannel](configs.md#logchannel)
* [getUpdates](configs.md#getupdates)

## JoinLeaveMessage

* [joinMessage](configs.md#joinmessage)
* [joinMessageChannel](configs.md#joinmessagechannel)
* [leaveMessage](configs.md#leavemessage)
* [leaveMessageChannel](configs.md#leavemessagechannel)

## Invites

* [autoSubtractFakes](configs.md#autosubtractfakes)
* [autoSubtractLeaves](configs.md#autosubtractleaves)
* [autoSubtractLeaveThreshold](configs.md#autosubtractleavethreshold)

## Ranks

* [rankAssignmentStyle](configs.md#rankassignmentstyle)
* [rankAnnouncementChannel](configs.md#rankannouncementchannel)
* [rankAnnouncementMessage](configs.md#rankannouncementmessage)

## Leaderboard

* [leaderboardStyle](configs.md#leaderboardstyle)
* [hideLeftMembersFromLeaderboard](configs.md#hideleftmembersfromleaderboard)

## Captcha

* [captchaVerificationOnJoin](configs.md#captchaverificationonjoin)
* [captchaVerificationWelcomeMessage](configs.md#captchaverificationwelcomemessage)
* [captchaVerificationSuccessMessage](configs.md#captchaverificationsuccessmessage)
* [captchaVerificationFailedMessage](configs.md#captchaverificationfailedmessage)
* [captchaVerificationTimeout](configs.md#captchaverificationtimeout)
* [captchaVerificationLogEnabled](configs.md#captchaverificationlogenabled)

## Moderation

* [mutedRole](configs.md#mutedrole)
* [modLogChannel](configs.md#modlogchannel)
* [modPunishmentBanDeleteMessage](configs.md#modpunishmentbandeletemessage)
* [modPunishmentKickDeleteMessage](configs.md#modpunishmentkickdeletemessage)
* [modPunishmentSoftbanDeleteMessage](configs.md#modpunishmentsoftbandeletemessage)
* [modPunishmentWarnDeleteMessage](configs.md#modpunishmentwarndeletemessage)
* [modPunishmentMuteDeleteMessage](configs.md#modpunishmentmutedeletemessage)
* [autoModEnabled](configs.md#automodenabled)
* [autoModModeratedChannels](configs.md#automodmoderatedchannels)
* [autoModModeratedRoles](configs.md#automodmoderatedroles)
* [autoModIgnoredChannels](configs.md#automodignoredchannels)
* [autoModIgnoredRoles](configs.md#automodignoredroles)
* [autoModDeleteBotMessage](configs.md#automoddeletebotmessage)
* [autoModDeleteBotMessageTimeoutInSeconds](configs.md#automoddeletebotmessagetimeoutinseconds)
* [autoModLogEnabled](configs.md#automodlogenabled)
* [autoModDisabledForOldMembers](configs.md#automoddisabledforoldmembers)
* [autoModDisabledForOldMembersThreshold](configs.md#automoddisabledforoldmembersthreshold)
* [autoModDisabledForOldMembersReceiveSilentWarning](configs.md#automoddisabledforoldmembersreceivesilentwarning)
* [autoModInvitesEnabled](configs.md#automodinvitesenabled)
* [autoModLinksEnabled](configs.md#automodlinksenabled)
* [autoModLinksWhitelist](configs.md#automodlinkswhitelist)
* [autoModLinksBlacklist](configs.md#automodlinksblacklist)
* [autoModLinksFollowRedirects](configs.md#automodlinksfollowredirects)
* [autoModWordsEnabled](configs.md#automodwordsenabled)
* [autoModWordsBlacklist](configs.md#automodwordsblacklist)
* [autoModAllCapsEnabled](configs.md#automodallcapsenabled)
* [autoModAllCapsMinCharacters](configs.md#automodallcapsmincharacters)
* [autoModAllCapsPercentageCaps](configs.md#automodallcapspercentagecaps)
* [autoModDuplicateTextEnabled](configs.md#automodduplicatetextenabled)
* [autoModDuplicateTextTimeframeInSeconds](configs.md#automodduplicatetexttimeframeinseconds)
* [autoModQuickMessagesEnabled](configs.md#automodquickmessagesenabled)
* [autoModQuickMessagesNumberOfMessages](configs.md#automodquickmessagesnumberofmessages)
* [autoModQuickMessagesTimeframeInSeconds](configs.md#automodquickmessagestimeframeinseconds)
* [autoModMentionUsersEnabled](configs.md#automodmentionusersenabled)
* [autoModMentionUsersMaxNumberOfMentions](configs.md#automodmentionusersmaxnumberofmentions)
* [autoModMentionRolesEnabled](configs.md#automodmentionrolesenabled)
* [autoModMentionRolesMaxNumberOfMentions](configs.md#automodmentionrolesmaxnumberofmentions)
* [autoModEmojisEnabled](configs.md#automodemojisenabled)
* [autoModEmojisMaxNumberOfEmojis](configs.md#automodemojismaxnumberofemojis)

## Detailed Config Options

### prefix

The prefix needed to use bot commands. If you don't remember your prefix, you can do @InviteManager config prefix

Type: `String`

Default: `!`

**Configuration**

Reset to default: `!config prefix default`

Examples:

`!config prefix +`

`!config prefix >`

### lang

Set the language of the bot

Type: `String`
Yo 
Default: `en`

**Configuration**

Reset to default: `!config lang default`

Possible values: `de`, `en`, `es`, `fr`, `it`, `nl`, `pt`, `ro`, `sv`

Example:

`!config lang de`

### logChannel

The channel where changes to the database are made \(add-ranks, clear-invites, etc.\)

Type: `Channel`

Default: `null`

**Configuration**

Reset to default: `!config logChannel default`
Examples:

`!config logChannel #channel`

### getUpdates

Whether or not you want to receive updates of our bot in the log or mod channel.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config getUpdates default`

Enable:

`!config getUpdates true`

Disable:

`!config getUpdates false`

### joinMessage

The message that will be posted every time a member joins your server.

Type: `String`

Default: `{memberMention} **joined**; Invited by **{inviterName}** (**{numInvites}** invites)`

**Configuration**

Reset to default: `!config joinMessage default`

Examples:

`!config joinMessage`

`!config joinMessage`

{% hint style="info" %}
Premium users can use embeds as join messages.
{% endhint %}

### joinMessageChannel

The channel where join messages will be posted.

Type: `Channel`

Default: `null`

**Configuration**

Reset to default: `!config joinMessageChannel default`

Examples:

`!config joinMessageChannel #general`

`!config joinMessageChannel #joins`

### leaveMessage

The message that will be posted every time a member leaves your server.

Type: `String`

Default: `{memberName} **left**; Invited by **{inviterName}**`

**Configuration**

Reset to default: `!config leaveMessage default`

Examples:

`!config leaveMessage`

`!config leaveMessage`

{% hint style="info" %}
Premium users can use embeds as leave messages.
{% endhint %}

### leaveMessageChannel

The channel where leave messages will be posted.

Type: `Channel`

Default: `null`

**Configuration**

Reset to default: `!config leaveMessageChannel default`

Examples:

`!config leaveMessageChannel #general`

`!config leaveMessageChannel #leaves`

### leaderboardStyle

Change the style how the leaderboard is displayed.

Type: `String`

Default: `normal`

**Configuration**

Reset to default: `!config leaderboardStyle default`

Possible values: `normal`, `table`, `mentions`

Example:

`!config leaderboardStyle normal`

### hideLeftMembersFromLeaderboard

Whether or not to hide people who left from the leaderboard.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config hideLeftMembersFromLeaderboard default`

Enable:

`!config hideLeftMembersFromLeaderboard true`

Disable:

`!config hideLeftMembersFromLeaderboard false`

### autoSubtractFakes

Should fake invites automatically be subtracted from invites?

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoSubtractFakes default`

Enable:

`!config autoSubtractFakes true`

Disable:

`!config autoSubtractFakes false`

### autoSubtractLeaves

Should members who leave be subtracted from their inviters?

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoSubtractLeaves default`

Enable:

`!config autoSubtractLeaves true`

Disable:

`!config autoSubtractLeaves false`

### autoSubtractLeaveThreshold

The time \(in seconds\) within leaves will be subtracted from the inviter.
Type: `Number`

Default: `600`

**Configuration**

Reset to default: `!config autoSubtractLeaveThreshold default`

Examples:

`!config autoSubtractLeaveThreshold 60`

`!config autoSubtractLeaveThreshold 3600`

### rankAssignmentStyle

If set to `highest`, only the highest rank will assigned to the member when reaching a new rank.If set to `all`, all ranks will be assigned to the member when reaching a new rank.

Type: `String`

Default: `all`

**Configuration**

Reset to default: `!config rankAssignmentStyle default`

Possible values: `all`, `highest`

Example:

`!config rankAssignmentStyle all`

### rankAnnouncementChannel

The channel where rank changes are announced.

Type: `Channel`

Default: `null`

**Configuration**

Reset to default: `!config rankAnnouncementChannel default`

Examples:

`!config rankAnnouncementChannel`

`!config rankAnnouncementChannel`

### rankAnnouncementMessage

The message that will be posted when a member reaches a new rank.

Type: `String`

Default: `Congratulations, **{memberMention}** has reached the **{rankName}** rank!`

**Configuration**

Reset to default: `!config rankAnnouncementMessage default`

Examples:

`!config rankAnnouncementMessage`

`!config rankAnnouncementMessage`

{% hint style="info" %}
Premium users can use embeds as rank announcement messages.
{% endhint %}

### mutedRole

The role that will be assigned if a member is muted by the bot

Type: `Role`

Default: `null`

**Configuration**

Reset to default: `!config mutedRole default`

Examples:

`!config mutedRole @muted`

### captchaVerificationOnJoin

If enabled, new members have to verify they are human by entering a captcha that is sent to them via DM. If they fail to enter the captcha within the specified time, they will be kicked from the server.

Type: `Boolean`

Default: `false`

**Configuration**

Reset to default: `!config captchaVerificationOnJoin default`

Enable:

`!config captchaVerificationOnJoin true`

Disable:

`!config captchaVerificationOnJoin false`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### captchaVerificationWelcomeMessage

The message users receive together with the captcha \(via DM\)

Type: `String`

Default: `Welcome to the server **{serverName}**! For extra protection, new members are required to enter a captcha.`

**Configuration**

Reset to default: `!config captchaVerificationWelcomeMessage default`

Examples:

`!config captchaVerificationWelcomeMessage Welcome, please enter the captcha below!`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### captchaVerificationSuccessMessage

The message users will get after successfully entering the captcha.

Type: `String`

Default: `You have successfully entered the captcha. Welcome to the server!`

**Configuration**

Reset to default: `!config captchaVerificationSuccessMessage default`

Examples:

`!config captchaVerificationSuccessMessage Thanks for entering the captcha, enjoy our server!`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### captchaVerificationFailedMessage

The message users will get if they fail to enter the right captcha within the specified time. After getting this message, they will be kicked from the server.

Type: `String`

Default: `You did not enter the captha right within the specified time.We're sorry, but we have to kick you from the server. Feel free to join again.`

**Configuration**

Reset to default: `!config captchaVerificationFailedMessage default`

Examples:

`!config captchaVerificationFailedMessage Looks like you are not human :(. You can join again and try again later if this was a mistake!`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### captchaVerificationTimeout

The time within the member needs to enter the captcha successfully \(in seconds\).

Type: `Number`

Default: `180`

**Configuration**

Reset to default: `!config captchaVerificationTimeout default`

Examples:

`!config captchaVerificationTimeout 60`


`!config captchaVerificationTimeout 600`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### captchaVerificationLogEnabled

Whether or not new captcha entries are logged to a channel

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config captchaVerificationLogEnabled default`

Enable:

`!config captchaVerificationLogEnabled true`

Disable:

`!config captchaVerificationLogEnabled false`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### modLogChannel

The channel where moderation log messages will be posted.

Type: `Channel`

Default: `null`

**Configuration**

Reset to default: `!config modLogChannel default`

Examples:

`!config modLogChannel #channel`

`!config modLogChannel #logs`

### modPunishmentBanDeleteMessage

Whether or not the own and bot message should be deleted when a mod does !ban.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config modPunishmentBanDeleteMessage default`

Enable:

`!config modPunishmentBanDeleteMessage true`

Disable:

`!config modPunishmentBanDeleteMessage false`

### modPunishmentKickDeleteMessage

Whether or not the own and bot message should be deleted when a mod does !kick.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config modPunishmentKickDeleteMessage default`

Enable:

`!config modPunishmentKickDeleteMessage true`

Disable:

`!config modPunishmentKickDeleteMessage false`

### modPunishmentSoftbanDeleteMessage

Whether or not the own and bot message should be deleted when a mod does !softban.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config modPunishmentSoftbanDeleteMessage default`

Enable:

`!config modPunishmentSoftbanDeleteMessage true`

Disable:

`!config modPunishmentSoftbanDeleteMessage false`

### modPunishmentWarnDeleteMessage

Whether or not the own and bot message should be deleted when a mod does !warn.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config modPunishmentWarnDeleteMessage default`

Enable:

`!config modPunishmentWarnDeleteMessage true`

Disable:

`!config modPunishmentWarnDeleteMessage false`

### modPunishmentMuteDeleteMessage

Whether or not the own and bot message should be deleted when a mod does !mute.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config modPunishmentMuteDeleteMessage default`

Enable:

`!config modPunishmentMuteDeleteMessage true`

Disable:

`!config modPunishmentMuteDeleteMessage false`

### autoModEnabled

Whether or not auto-moderation is enabled globally.

Type: `Boolean`

Default: `false`

**Configuration**

Reset to default: `!config autoModEnabled default`

Enable:

`!config autoModEnabled true`

Disable:

`!config autoModEnabled false`

### autoModModeratedChannels

Set channels that should be auto-moderated. \(Comma separated list\)

Type: `List of Channel`

Default: `null`


**Configuration**

Reset to default: `!config autoModModeratedChannels default`

Examples:

`!config autoModModeratedChannels #general`

`!config autoModModeratedChannels #support,#help`

### autoModModeratedRoles

Roles that will be auto-moderated. \(Comma separated list\)

Type: `List of Role`

Default: `null`

**Configuration**

Reset to default: `!config autoModModeratedRoles default`

Examples:

`!config autoModModeratedRoles @NewMembers`

`!config autoModModeratedRoles @Newbies,@Starters`

### autoModIgnoredChannels

Set channels that should not be auto-moderated. \(Comma separated list\)

Type: `List of Channel`

Default: `null`

**Configuration**

Reset to default: `!config autoModIgnoredChannels default`

Examples:

`!config autoModIgnoredChannels #general`

`!config autoModIgnoredChannels #off-topic,#nsfw`

### autoModIgnoredRoles

Roles that will not be auto-moderated. \(Comma separated list\)

Type: `List of Role`

Default: `null`

**Configuration**

Reset to default: `!config autoModIgnoredRoles default`


Examples:

`!config autoModIgnoredRoles @TrustedMembers`

`!config autoModIgnoredRoles @Moderators,@Staff`

### autoModDeleteBotMessage

Whether or not to delete bot messages after auto-moderation.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModDeleteBotMessage default`

Enable:

`!config autoModDeleteBotMessage true`

Disable:

`!config autoModDeleteBotMessage false`

### autoModDeleteBotMessageTimeoutInSeconds

How long \(in seconds\) until auto-moderation responses from the bot are deleted. If set to 0, the bot will not post a message and only delete the violating message and warn the user.

Type: `Number`

Default: `5`

**Configuration**

Reset to default: `!config autoModDeleteBotMessageTimeoutInSeconds default`

Examples:

`!config autoModDeleteBotMessageTimeoutInSeconds 5`

`!config autoModDeleteBotMessageTimeoutInSeconds 10`

### autoModLogEnabled

If set to yes, all moderation actions will be logged to the `modLogChannel`.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModLogEnabled default`

Enable:

`!config autoModLogEnabled true`

Disable:

`!config autoModLogEnabled false`

### autoModDisabledForOldMembers

If enabled, members that have been on the server for a certain amount of time will not be auto-moderated. You can set the threshold for how long that is.

Type: `Boolean`

Default: `false`

**Configuration**

Reset to default: `!config autoModDisabledForOldMembers default`

Enable:

`!config autoModDisabledForOldMembers true`

Disable:

`!config autoModDisabledForOldMembers false`

### autoModDisabledForOldMembersThreshold

After how long \(in seconds\) members will no longer be auto-moderated \(if enabled\).

Type: `Number`

Default: `604800`

**Configuration**

Reset to default: `!config autoModDisabledForOldMembersThreshold default`

Examples:

`!config autoModDisabledForOldMembersThreshold 604800` \(1 week\)\`\`

`!config autoModDisabledForOldMembersThreshold 2419200` \(1 month\)\`\`

### autoModDisabledForOldMembersReceiveSilentWarning

If enabled, old members will still receive a warning via DM when violating a rule.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModDisabledForOldMembersReceiveSilentWarning default`

Enable:

`!config autoModDisabledForOldMembersReceiveSilentWarning true`

Disable:

`!config autoModDisabledForOldMembersReceiveSilentWarning false`

### autoModInvitesEnabled

If enabled, invite links will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModInvitesEnabled default`

Enable:

`!config autoModInvitesEnabled true`

Disable:

`!config autoModInvitesEnabled false`

### autoModLinksEnabled

If enabled, links will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModLinksEnabled default`


Enable:

`!config autoModLinksEnabled true`

Disable:

`!config autoModLinksEnabled false`

### autoModLinksWhitelist

A comma separated list of links that are allowed to be posted.

Type: `List of String`

Default: `null`

**Configuration**

Reset to default: `!config autoModLinksWhitelist default`

Examples:

`!config autoModLinksWhitelist discordbots.org`

`!config autoModLinksWhitelist youtube.com,twitch.com`

### autoModLinksBlacklist

A comma separated list of links that are not allowed to be posted.

Type: `List of String`

Default: `null`

**Configuration**

Reset to default: `!config autoModLinksBlacklist default`

Examples:

`!config autoModLinksBlacklist google.com`

`!config autoModLinksBlacklist twitch.com,youtube.com`

### autoModLinksFollowRedirects

If enabled, our bot will follow redirects to see where a link leads \(to prevent people from using link-shorteners.\)

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModLinksFollowRedirects default`

Enable:

`!config autoModLinksFollowRedirects true`

Disable:

`!config autoModLinksFollowRedirects false`

{% hint style="info" %}
This feature is only available for premium users.
{% endhint %}

### autoModWordsEnabled

If enabled, certain words will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModWordsEnabled default`

Enable:

`!config autoModWordsEnabled true`

Disable:

`!config autoModWordsEnabled false`

### autoModWordsBlacklist

A comma separated list of words that will be auto-moderated.

Type: `List of String`

Default: `null`

**Configuration**

Reset to default: `!config autoModWordsBlacklist default`

Examples:

`!config autoModWordsBlacklist gay`

`!config autoModWordsBlacklist stupid,fuck`

### autoModAllCapsEnabled

If enabled, messages written in all/mostly CAPS will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModAllCapsEnabled default`

Enable:

`!config autoModAllCapsEnabled true`

Disable:

`!config autoModAllCapsEnabled false`

### autoModAllCapsMinCharacters

How long a message needs to be until this violation is activated.

Type: `Number`

Default: `10`

**Configuration**

Reset to default: `!config autoModAllCapsMinCharacters default`

Examples:

`!config autoModAllCapsMinCharacters 5`

`!config autoModAllCapsMinCharacters 15`

### autoModAllCapsPercentageCaps

Percentage of letters that need to be CAPS to be triggered.

Type: `Number`

Default: `70`

**Configuration**

Reset to default: `!config autoModAllCapsPercentageCaps default`

Examples:

`!config autoModAllCapsPercentageCaps 50`

`!config autoModAllCapsPercentageCaps 90`

### autoModDuplicateTextEnabled

If enabled, duplicate text will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModDuplicateTextEnabled default`

Enable:

`!config autoModDuplicateTextEnabled true`

Disable:

`!config autoModDuplicateTextEnabled false`

### autoModDuplicateTextTimeframeInSeconds

Time \(in seconds\) within the same text of the same author will be auto-moderated.

Type: `Number`

Default: `60`

**Configuration**

Reset to default: `!config autoModDuplicateTextTimeframeInSeconds default`

Examples:

`!config autoModDuplicateTextTimeframeInSeconds 5`

`!config autoModDuplicateTextTimeframeInSeconds 20`

### autoModQuickMessagesEnabled

If enabled, message sent quickly after another will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModQuickMessagesEnabled default`

Enable:

`!config autoModQuickMessagesEnabled true`

Disable:

`!config autoModQuickMessagesEnabled false`

### autoModQuickMessagesNumberOfMessages

How many messages within the specified amount of time will be considered spam and are auto-moderated.

Type: `Number`

Default: `5`


**Configuration**

Reset to default: `!config autoModQuickMessagesNumberOfMessages default`

Examples:

`!config autoModQuickMessagesNumberOfMessages 5`

`!config autoModQuickMessagesNumberOfMessages 10`

### autoModQuickMessagesTimeframeInSeconds

During what timeframe \(in seconds\) quick messages will be counted.

Type: `Number`

Default: `3`

**Configuration**

Reset to default: `!config autoModQuickMessagesTimeframeInSeconds default`

Examples:

`!config autoModQuickMessagesTimeframeInSeconds 2`

`!config autoModQuickMessagesTimeframeInSeconds 10`

### autoModMentionUsersEnabled

If enabled, too many user mentions will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModMentionUsersEnabled default`

Enable:

`!config autoModMentionUsersEnabled true`

Disable:

`!config autoModMentionUsersEnabled false`

### autoModMentionUsersMaxNumberOfMentions

Maximum amount of user mentions per message.

Type: `Number`

Default: `5`

**Configuration**

Reset to default: `!config autoModMentionUsersMaxNumberOfMentions default`

Examples:

`!config autoModMentionUsersMaxNumberOfMentions 2`

`!config autoModMentionUsersMaxNumberOfMentions 5`

### autoModMentionRolesEnabled

If enabled, too many role mentions will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModMentionRolesEnabled default`

Enable:

`!config autoModMentionRolesEnabled true`

Disable:

`!config autoModMentionRolesEnabled false`

### autoModMentionRolesMaxNumberOfMentions

Maximum amount of role mentions per message.

Type: `Number`

Default: `3`

**Configuration**

Reset to default: `!config autoModMentionRolesMaxNumberOfMentions default`

Examples:

`!config autoModMentionRolesMaxNumberOfMentions 2`

`!config autoModMentionRolesMaxNumberOfMentions 5`

### autoModEmojisEnabled

If enabled, too many emojis will be auto-moderated.

Type: `Boolean`

Default: `true`

**Configuration**

Reset to default: `!config autoModEmojisEnabled default`

Enable:

`!config autoModEmojisEnabled true`

Disable:

`!config autoModEmojisEnabled false`

### autoModEmojisMaxNumberOfEmojis

Maximum amount of emojis per message.

Type: `Number`

Default: `5`

**Configuration**

Reset to default: `!config autoModEmojisMaxNumberOfEmojis default`

Examples:

`!config autoModEmojisMaxNumberOfEmojis 5`

`!config autoModEmojisMaxNumberOfEmojis 10` 
