# What is it?
Auto-Respawn for 1.12.2 is a client-side mod that works on both Singleplayer and Multiplayer worlds
/autorespawn, /ar, or /respawn can be used to toggle the auto-respawn functionality.
# Credits
The initial idea was put forth by u/boxtopy in a post on r/feedthebeast. (https://www.reddit.com/r/feedthebeast/comments/e3xtwf/auto_respawn_mod_for_1122/)
# Misc
Feel free to use this mod however you like, whether it be in a modpack or otherwise.
# A note/story from me
My freind asked me how to build this plugin. Of course, I couldn't not help him, so I have taken a look on repository, and said "I can try building it, but I don't know will it work..".

The first build with gradlew was fine. I have executed "gradlew.bat" and it returned "BUILD SUCCESFUL".
But also, I didn't saw any JAR file... Only BIN..

And I went to Google. I have found this article: https://mcforge.readthedocs.io/en/latest/gettingstarted/ , that said:
```To build your mod, run gradlew build. This will output a file in build/libs with the name [archivesBaseName]-[version].jar. This file can be placed in the mods folder of a Forge enabled Minecraft setup or distributed.```
Amazing! Now we need to run gradlew build.. and build failed. Why?

Because gradlew couldn't find a library, but, it said that I need to install JDK. I did not had it installed so..  I've tried downloading it from Oracle.  But, it refused to download with error,
that basically said "This site .../jdk-8u311-windows-x64.exe is experiencing technical difficulty. We are aware of the issue and are working as quick as possible to correct the issue."

Well, because of current situation a lot of websites and services refused to work in Russia. So, I tried with VPN, and surely, it downloaded.

Anyways, after installing jdk it still couldn't find it..

I removed my Java 8(JRE), and added some things in env. vars in Windows.

Now, the build was succesful! And in build/libs I have found an JAR file that I've sent to my freind.
