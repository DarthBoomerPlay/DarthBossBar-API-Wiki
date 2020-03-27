# DarthBossBar-API-Wiki
Spigot: https://www.spigotmc.org/resources/darthbossbar.76557/
\
### My Links:
    Discord: DarthBoomerPlay#6534
    VK: https://vk.com/darthboomerplay
    Donation link: https://donationalerts.com/r/darthboomerplay_
  

# Adding DarthBossBar to your project

##  Manual:
   If you want to manually add the API dependency to your classpath, you can obtain the jar by:
    
    1. Navigating to https://www.spigotmc.org/resources/darthbossbar.76557/
    2. Download plugin and added to your classpath.
    
# Obtaining an instance of the API
   When the plugin is enabled, an instance of DarthBossBarAPI can be obtained using this method:
```java
public DarthBossBarAPI api;

public void onEnable()
{
    api = new DarthBossBarAPI();
}
```
\
   Currently API contains these functions:
```java
public List<BossBarInfo> getBossBars() // returns bossbars list
public BossBarInfo getBossBar(int id) // returns bossbar

public void addBossBar(BarColor color, BarStyle style, String message, int seconds) // creates bossbar
public void removeBossBar(int id) // deletes bossbar
```
\
   BossBarInfo contains:
```java
public int getID() // get bossbar ID

public BarColor getColor() // gets the color of the bossbar
public void setColor(BarColor color) // sets the bossbar color

public BarStyle getStyle() // gets the bossbar style
public void setStyle(BarStyle style) // sets the bossbar style

public String getMessage() // gets the message text
public void setMessage(String message) // sets the message text

public int getSecondsTime() // gets time in seconds
public void setSecondsTime(int seconds) // sets time in seconds
```
