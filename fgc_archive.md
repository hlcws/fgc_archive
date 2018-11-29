# Idea

Data related to FGC events should be stored in an universal archive that can be accessed/replicated/contributed by anyone. Storing data in proprietary formats on commercial and potentially short-lived providers leads to data loss, e.g. storing a tournament bracket as JPG screenshot on Imgbanana or Yahoo.

This is independent from the presentation for end-users, they should still be able to conveniently access photos via facebook/twitter/etc.

The Data package should be universal so that it can be stores on FTP, HTTP, GIT, Google Drive, etc.
This way anyone can run their own repository. Different repositories should be merge-able. Some definitions should be truly global, e.g. game names and character abbreviations.

Tools should be built based on this suggested structure to submit, extract data and generate simple viewers, e.g.
- PHP upload form for photos
- Dump twitch archive and highlights into mp4
- Generate HTML gallery (Jekyll?)

Distribution via GIT, Torrent, Blockchain, ...

# Content

- File based storage for media (photos, videos)
- Metadata as plain text
- Event coverage as markdown/screenshot (articles, tweets, posts, ...)
- Plain HTML for offline viewing (e.g. Jekyll with gallery generator)

# File Names

File names should be human readable and friendly, yet parseable. Verify with regex before submitting.

# Suggestion/Examples

File Structure suggestion/examples:

Definitions\

Definitions\Games\

Definitions\Games\Soul_Calibur_VI.txt

- Friendly name, Alias
- Character names, abbreviations, alias

Year\Year-Month-Day-Eventname-Location\

Year\Year-Month-Day-Eventname-Location\bracket-top64.png

Year\Year-Month-Day-Eventname-Location\bracket-top64.txt

- matches containt player names, characters, scores and parent matches
- matches have 2 fathers
- bracket should be rebuildable from this dump

2018\2018-11-30-Tekken-World-Tour-EU-NL-Amsterdam\Description.txt
- Event Name
- Date
- Location
- Games

Year\Year-Month-Day-Eventname-Location\Media\

Year\Year-Month-Day-Eventname-Location\Media\Photos\Eventname_date_location_suffix.jpg
- jpg
- png
- gif
- gfy

Year\Year-Month-Day-Eventname-Location\Media\Videos\

Year\Year-Month-Day-Eventname-Location\Media\Videos\Eventname_date_location_game_bracket.mp4

Year\Year-Month-Day-Eventname-Location\Media\Videos\Eventname_date_location_game_bracket.txt
- Timestamps
- Player names
- Characters (database with accepted names??)
- Score
