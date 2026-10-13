# Reworked Spotify [MAC]

A minimal, outlined dark rework of Spotify, built on the Subtle Outline theme. Every page uses the same look: thin outlined boxes, flat dark background, compact rows and no gradients. Only for macOS.

![Reworked Spotify preview](images/preview.png)

## Features

### Everything from Subtle Outline
- **Boxed top bar**: back, forward and Home in one box; a full-width search bar; settings, Browse, Marketplace, What's New, Listening activity and your profile on the right.
- **Room for the macOS window buttons**, which stays correct when you resize the window.
- **Colour schemes** (all dark): Subtle (default), Midnight, Forest, Ember, Amethyst and Mono, plus Simple Outline's Natural and Droid.

### Home
- A big **Liked Songs** tile (collage of your latest likes, Play, Shuffle and DJ) beside your shortcuts.
- **Recents** that update live, including single songs you played from search or Liked Songs.
- **Quick picks**: your recently liked songs as compact rows.
- Spotify's rows as tidy one-row boxes; the rest folds under **More for you**.
- The **All / Music / Podcasts / Audiobooks** chips change what's shown (no Liked Songs under Podcasts, and so on).

### Artist pages
- Compact header with a round picture and **Read bio**.
- One box of equal icon buttons: Play, Shuffle, Follow, **Wikipedia**, More.
- **Popular** always shows 10 songs.
- **Discography** lists every release and can **search songs inside albums** ("On Sight" finds it on Yeezus).
- **Wikipedia panel**: the artist's article in a dark, readable layout with contents and details. Also in the right-click menu on any artist.

### Playlists, albums, Liked Songs, Local Files and profiles
- Flat header with the cover, outlined toolbar, small chips, and the track list and Recommended in outlined boxes.

### Everywhere
- Pop-up menus, tooltips and the Now Playing panel in the theme's colours.
- The **DJ** in black and white: a static white DJ mark instead of the animated green visual.
- Light on resources: no animations running in the background, and page styling only runs when a page changes, so it suits low-end and battery-powered laptops.

### Settings (paintbrush icon, top right)
Everything from Subtle Outline (corners, colours, outline thickness, top bar options), plus:
- **Home**: Quick picks on/off; how many rows show before "More for you" (2, 3, 5 or All).
- **Artist page**: show extra sections (You Liked, Artist pick, On Tour, Fans also like and the rest).
- **Reset to defaults** resets all of it.

## Install

Install **Reworked Spotify** from the Themes tab in [Spicetify Marketplace](https://github.com/spicetify/marketplace). It's tagged "external JS" because it includes `reworked-spotify.js`, which provides the layouts and the settings panel.

Don't run it together with Subtle Outline; this theme already includes it.

### Manual install

1. Copy `user.css` and `color.ini` into `~/.config/spicetify/Themes/Reworked Spotify/`.
2. Copy `reworked-spotify.js` into `~/.config/spicetify/Extensions/`.
3. Run:
   ```
   spicetify config current_theme "Reworked Spotify" color_scheme Subtle
   spicetify config extensions reworked-spotify.js
   spicetify apply
   ```

## Notes

- Made for **macOS** only.
- Lyrics aren't part of this theme. It works well alongside [Spicy Lyrics](https://github.com/Spikerko/spicy-lyrics).
- The Wikipedia panel loads articles from wikipedia.org and wikidata.org when you open it. Nothing else is sent anywhere.
- Spotify updates sometimes rename the parts of the app this theme styles. Pages then fall back to Spotify's normal look rather than breaking. If something looks wrong after an update, please open an issue.
- After a Spotify update wipes Spicetify, run `spicetify backup apply`. Your settings are kept.

## Credits

- **Simple Outline** by [Droidiar](https://github.com/Droidiar): the original outlined theme (`user.css` and the Natural and Droid colour schemes).
- **Subtle Outline** and **Reworked Spotify** by [terminalsilliness](https://github.com/terminalsilliness).
- Wikipedia text is available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
