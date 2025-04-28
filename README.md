# Perfect Tower by Hypnocat Studios - Wiki

The `[local]` links only work if you have downloaded the [Google Drive folder](https://drive.google.com/drive/folders/12Y8So82ErUaTq831rcTpS4zghOwL0osP)!

To get a local copy of this wiki, download the GitHub repository. If you'd like the large media files too, download the [Google Drive folder](https://drive.google.com/drive/folders/12Y8So82ErUaTq831rcTpS4zghOwL0osP) and move all the video files into the "media" folder. Then you can use the `[local]` links to access the local media files.

## Upgrades

Once an upgrade has been bought, the player cannot undo it without using [editing the data file](#editing-the-data-file). Or you can delete and re-install the game to reset your progress.

| number* | cost in stars | what it does                                                    |
| ------- | ------------- | --------------------------------------------------------------- |
| 0       | 15            | adds water underneath the platform                              |
| 1       | 20            | adds a house on an island to the left of the platform           |
| 2       | 30            | darkens the platform and adds grass on it                       |
| 3       | 50            | adds a brown bird that stands on the right half of the platform |
| 4       | 70            | adds clouds                                                     |
| 5       | 90            | adds a hot air balloon                                          |
| 6       | 110           | adds a thin tower besides the house                             |
| 7       | 130           | adds a sailboat                                                 |
| 8       | 150           | adds a blimp                                                    |
| 9       | 170           | changes the platform to textured stone with messy grass         |
| 10      | 190           | adds dark blue flying birds (pigeons?)                          |
| 11      | 210           | adds a moon in the sky                                          |
| 12      | 230           | changes the house's tower to a wider red and white striped one  |
| 13      | 250           | adds a clownfish in the water                                   |
| 14      | 280           | adds low clouds/fog in the background                           |
| 15      | 310           | adds a green bird that stands on the left half of the platform  |
| 16      | 330           | adds flying seagulls                                            |
| 17      | 350           | adds a beige ringed planet                                      |
| 18      | 370           | adds a shark in the water                                       |
| 19      | 390           | changes the platform to a tree                                  |
| 20      | 410           | changes the lighthouse to a grey tower-house complex            |
| 21      | 430           | changes the sailboat to a steamboat                             |
| 22      | 450           | adds an astronaut attached to a satellite                       |
| 23      | 470           | changes the platform to the top of a Greek/Roman pillar         |
| 24      | -             | the upgrade button is not clickable                             |


\* as stated on the up arrow of the upgrade button

For graphics of what each upgrade looks like, refer to these videos:
- [All upgrades (dark mode)](https://drive.google.com/file/d/17XH7ztmresmT3fyMdexK2V1RJ8pLXgB8/), [\[local\]](media/all-upgrades-dark-mode.mp4)
- [All upgrades (light mode)](https://drive.google.com/file/d/1QI2LZ7Ob01nVmcZ-AaYELE8iTtuvdeI-/), [\[local\]](media/all-upgrades-light-mode.mp4)

## Cheats

### autoclicker

If you download an autoclicker app and run it to click once per second on the screen, and leave it running for a while, you will end up with more stars without having to play the game. I used the 'basic' mode of [Klick'r - Smart AutoClicker](https://github.com/Nain57/Smart-AutoClicker)

### editing the data file

The below method only works for Android and requires root permissions. If you don't have root permissions and would still like to proceed, there's a [nice guide for how to "root your phone"](https://topjohnwu.github.io/Magisk/install.html). If you don't know what root permissions are, then you likely don't have them.

Shut down the Perfect Tower app by going to Android's recents and then swiping it out.

Open this file in a text editor with root permissions: `/data/user/0/com.hypnocatstudio.perfecttower/shared_prefs/com.hypnocatstudio.perfecttower.v2.playerprefs.xml`

(`/data/user/0/com.hypnocatstudio.perfecttower/` is where Perfect Tower for your main Android profile stores its data. If you want to change the Perfect Tower save of a "second space" or "work profile", you might have to try `/data/user/10/com.hypnocatstudio.perfecttower/...`, or some other number after `/data/user/`. )

It will look like this
```xml
<?xml version='1.0' encoding='utf-8' standalone='yes' ?>
<map>
    <string name="CHALLENGES_COMPLETED">AQ%3D%3D</string>
    <int name="Screenmanager%20Resolution%20Height" value="1920" />
    <int name="UPGRADES_PURCHASED" value="23" />
    <int name="NIGHT_MODE" value="1" />
    <string name="unity.player_sessionid">532931913080811087</string>
    <int name="PAID_CHARACTER" value="0" />
    <int name="Screenmanager%20Resolution%20Width" value="1080" />
    <string name="DAILY_CHALLENGES_IDS">ASAAAAAOAAAAFAAAAA%3D%3D</string>
    <int name="CHALLENGES_PLAYED" value="0" />
    <int name="VISIT_DAYS_IN_A_ROW" value="1" />
    <int name="GAMES_PLAYED" value="2" />
    <int name="DAILY_REWARDS" value="1" />
    <int name="com.lionstudios.analytics.timeinapp" value="368" />
    <int name="BOOSTER_ROTATE" value="3" />
    <int name="NEED_SHOW_TUTORIAL" value="0" />
    <string name="UNLOCKED_FIGURES_PAID">AQ%3D%3D</string>
    <string name="Lion_LocationInfo">your-location</string>
    <string name="NEXT_DAYLY_CHALLENGE_TIME">-8584557886549533678</string>
    <string name="NEXT_DAILY_REWARD_TIME">638814816000000000</string>
    <string name="unity.player_session_count">3</string>
    <int name="HAS_ADS" value="0" />
    <string name="DAILY_CHALLENGES_COMPLETED">AgMAAAAA</string>
    <int name="CURRENT_SPECIAL_FIGURE_ID" value="0" />
    <int name="BOOSTER_RAINBOW" value="3" />
    <int name="SOUND_ON" value="1" />
    <int name="__UNITY_PLAYERPREFS_VERSION__" value="1" />
    <int name="BEST_SCORE" value="10" />
    <int name="BOOSTER_DROP" value="3" />
    <int name="VIBRATION_ENABLED" value="0" />
    <string name="unity.cloud_userid">a-hexadecimal-number</string>
    <int name="Screenmanager%20Fullscreen%20mode" value="1" />
    <int name="COINS" value="99295" />
    <string name="UNLOCKED_FIGURES">AQAAAAAEAAAAEAAAABIAAAAYAAAA</string>
</map>
```

Change the `value=` fields to change your in-game statistics.

| name               | what it is                                                                                                              |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| COINS              | the number of stars you have                                                                                            |
| UPGRADES_PURCHASED | the number of upgrades the background should be displayed with. Changing this value will not decrement your star count. |


Save the file. 

Open Perfect Tower. You should now see the cheated progress on screen!

## Special Shapes

[A video that shows the requirements to unlock each special shape](https://drive.google.com/file/d/1qHb5dJvYU6xwo-YptZJvM7kgqTeLHjWo/), [\[local\]](media/special-shapes-descriptions.mp4)
