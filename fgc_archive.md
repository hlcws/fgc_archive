Data related to FGC events should be stored in an universal archive that can be accessed/replicated/contributed by anyone. Storing data in proprietary formats on commercial and potentially short-lived providers leads to data loss, e.g. storing a tournament bracket as JPG screenshot on Imgbanana or Yahoo.

This is independent from the presentation for end-users, they should still be able to conveniently access photos via facebook/twitter/etc.

---
Suggestion:

File based storage for media (photos, videos)
Metadata as plain text
Event coverage as markdown/screenshot
Plain HTML for offline viewing (e.g. Jekyll)

Distribution via FTP, HTTP, torrent, blockchain, GIT, whatever

Should be mergable world-wide

Simple tools for submitting  data, e.g. batch files or PHP upload forms.

---
File names should be human readable and friendly, yet parseable. 

---

File Structure:
Definitions\
Definitions\Games\
Definitions\Games\Soul_Calibur_VI.txt
Friendly name, Alias
Character names, abbreviations, alias

Year\Year-Month-Day-Eventname-Location\
2018\2018-11-30-Hessen-Crash-XIV-Frankfurt\

Description.txt
Event Name
Date
Location
Games

Media\
Photos\
Eventname_date_location_suffix.jpg
*.jpg, *.png, *.gif

Videos\
Eventname_date_location_game_bracket.mp4
Eventname_date_location_game_bracket.txt
Timestamps
Player names
Characters (database with accepted names??)
Score


