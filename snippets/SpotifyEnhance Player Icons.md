# SpotifyEnhance Player Icons
Adds Icons to the Player Widget that Skamts SpotifyEnhance plugin adds.
(Also replaces the "by" for artists and "on" for albums with an icon that equally represents these fields)
> [!WARNING]
> Requires the following player settings:</br>
> Player Compact Mode must be **DISABLED**.</br>

 

## Installation
To install this snippet, simply copy the following CSS into your Custom CSS file:</br>
<details>
<summary>CSS</summary>

```css
.spotify-player-container {
  .spotify-player-media {
    margin-left: -5px;
    padding-right: 45px!important;
    width: 200px!important;
    overflow: hidden;
    padding: 5px;
    clip-path: inset(0);
  }
  .spotify-player-title {
    background-image: url("https://github.com/Riddim-GLiTCH/riddim-glitch.github.io/blob/main/assets/Icons/discord-import/quaver.png?raw=true");
    background-position: left;
    background-repeat: no-repeat;
    background-size: contain;
    padding-left: 22px;
    margin-left: -5px;
    color: black;
    filter: drop-shadow(0 0 1px white) invert(1);
  }
  .spotify-player-artist {
    width: 280px;
    background-image: url('https://github.com/Riddim-GLiTCH/riddim-glitch.github.io/blob/main/assets/Icons/discord-import/artist.png?raw=true');
    background-position: left;
    background-repeat: no-repeat;
    background-size: contain;
    padding-left: 20px;
    margin-left: -5px;
    filter: drop-shadow(0 0 1px white) invert(1);
  } 
  .spotify-player-album {
    background-image: url('https://github.com/Riddim-GLiTCH/riddim-glitch.github.io/blob/main/assets/Icons/discord-import/music-album.png?raw=true');
    background-position: left;
    background-repeat: no-repeat;
    background-size: contain;
    padding-left: 20px;
    margin-left: -5px;
    filter: drop-shadow(0 0 1px white) invert(1);
  }
  .spotify-player-artist, .spotify-player-album {
    font-size: 0;
    span {
      margin-left: -3px;
      font-size: small;
      margin-top: 5px;
      color: #45475a;
    }
  }
}
```
</details>

## Preview
![image](https://github.com/user-attachments/assets/42dd7799-285a-4f3c-b750-4bd2b98ff56b)

### Credit
@Riddim_GLiTCH

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

</details>
