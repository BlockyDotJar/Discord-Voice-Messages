[github-release-shield]: https://img.shields.io/github/v/release/BlockyDotJar/Discord-Voice-Messages
[github-release]: https://github.com/BlockyDotJar/Discord-Voice-Messages/releases/latest

[license-shield]: https://img.shields.io/badge/License-Apache%202.0-white.svg
[license]: https://github.com/BlockyDotJar/Discord-Voice-Messages/tree/main/LICENSE

[discord-invite-shield]: https://discord.com/api/guilds/876766868864647188/widget.png
[discord-invite]: https://discord.gg/mYKK4BwGxe

[concept]: #concept

# Discord Voice Messages


[ ![github-release-shield][] ][concept] [ ![license-shield][] ][license] [ ![discord-invite-shield][] ][discord-invite]

This is a Discord bot written in `Java` with the JDA (Java Discord API) library.
<p>At the moment i don't host this bot, but if you want to host it, you are allowed to do that.

## Summary

1. [Concept](#concept)
2. [Useful links](#useful-links)
3. [Requirements](#requirements)
4. [Contribution](#contribution)
5. [Dependencies](#dependencies)

## Concept

1. You are joining a specific `audio channel` (voice- or stagechannel) 
2. The bot joins the channel too
3. You say, whatever you have to say
4. You are leaving from the voice channel
5. The bot leaves the channel too
6. You are pinging the bot
7. The bot uploads the file to [Tixte](https://tixte.com/)
8. The bot sends a link to the file

## Useful links

* [JDA wiki](https://jda.wiki)
* [JDA-C wiki](https://github.com/BlockyDotJar/JDA-Commons/wiki)
* [Tixte4J wiki](https://github.com/BlockyDotJar/Tixte-Java-Library/wiki)
* [Getting started with Tixte4J](https://github.com/BlockyDotJar/Tixte-Java-Library/wiki/Getting-started)
* [Setting Tixte4J up](https://github.com/BlockyDotJar/Tixte-Java-Library/wiki/Setup)
* [Tixte4J troubleshooting](https://github.com/BlockyDotJar/Tixte-Java-Library/wiki/Troubleshooting)

## Requirements

* You have at least installed Java **19**
* A Discord bot token
* Your bot has access to following intents: `GUILD_VOICE_STATES`, `GUILD_MESSAGES` and `GUILD_MEMBERS`
* A Tixte API-key, session-token and default domain
* You have Gradle installed on your computer
* Basic Java, JDA and Tixte4J knowledge

## Contribution

If you want to contribute to this project, make sure to base your branch off of our **developer** branch
and create your PR into that **same** branch.
<br>**We will be rejecting any PRs, which are not based to the developer branch!**
<br>It is very possible that your change might already be in development or you missed something.

More information can be found at the [contributing](https://github.com/BlockyDotJar/Discord-Voice-Messages/wiki/Contributing) wiki page.

### Deprecation Policy

When a feature is introduced to replace or enhance existing functionality we might deprecate old functionality.

A deprecated method/class usually has a replacement mentioned in its documentation which should be switched to.
<br>Deprecated functionality might or might not exist in the next minor release. (Hint: The minor version is the `MM` of `XX.MM.RR(-TT.ZZ)` in our version format)

It is possible that some features are deprecated without replacement, in this case the functionality is no longer supported by either the Tixte4J/JDA(-C) structure
due to fundamental changes or due to Tixte-API/Discord-API changes that cause it to be removed.

We highly recommend discontinuing usage of deprecated functionality and update by going through each minor release instead of jumping.
<br>For instance, when updating from version `1.0.0-beta.1` to version `1.0.0-rc.2` you should do the following:

- Update to `1.0.0-beta.ZZ` and check for deprecation
- Update to `1.0.0-rc.2` and check for deprecation

The `RR` in version `1.0.RR` should be replaced by the latest version that was published for `1.0`, you can find out which the latest
version was by looking at the [release page](https://github.com/BlockyDotJar/Discord-VoiceMessages/releases)

## Dependencies

This project requires **Java 19+**
<br>All dependencies are managed automatically by Gradle.

* JDA
    * Version: **v5.0.0-beta.2**
    * [Github](https://github.com/DV8FromTheWorld/JDA)
* JDA-C
    * Version: **v1.2.1**
    * [Github](https://github.com/BlockyDotJar/JDA-Commons)
* Tixte4J
    * Version: **v1.1.8**
    * [Github](https://github.com/BlockyDotJar/Tixte-Java-Library)
* slf4j-api
    * Version: **v2.0.5**
    * [Github](https://github.com/qos-ch/slf4j)
* logback-classic
    * Version: **v1.4.5**
    * [Github](https://github.com/qos-ch/logback)
* jetbrains-annotations
    * Version: **v23.0.0**
    * [Github](https://github.com/JetBrains/java-annotations)
* error_prone_annotations
    * Version: **v2.16.0**
    * [Github](https://github.com/google/error-prone)

<hr>

These are only the libraries, which we have in our [build.gradle.kts](https://github.com/BlockyDotJar/Discord-Voice-Messages/blob/main/build.gradle.kts), but we are using [all libraries](https://github.com/DV8FromTheWorld/JDA#dependencies), which the original JDA uses too.

<hr>
