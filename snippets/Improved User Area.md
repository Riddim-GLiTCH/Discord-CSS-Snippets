# Improved User Area
Small improvements to the User Area. Displays your screen name, User Name and Status message all at once. Adds an @ to the username (Because apparently Discord doesn't know how usernames work 👍 )
Also hides the mute and deafen buttons until you hover over the settings button. (This is a modified version of the Hide User Buttons until Hover snippet by [@TheCommieAxolotl](https://github.com/TheCommieAxolotl))


## Installation
<details>
<summary>CSS</summary>

```css
/* --Improved User Area-- */
/* Make both the username and status message visible at all times. */
.container_b2ca13 .hovered_c0d6c6, .hoverRoll_c0d6c6.forceHover_c0d6c6:not(.disabled_c0d6c6) .default_c0d6c6{
  opacity: 1!important;
  transform: none;
}
/* Adds an @ to the username. Discord, for the love of god, just add this yourself already. */
.container_b2ca13 .hovered_c0d6c6::before{
  content: "@";
}
/* Move the custom Status message down so that it doesnt overlap with the Username */
.default_c0d6c6{
  margin-top: 15px;
}
/* Credit to @thecommieaxolotl for this code. */
/* --Hides User Buttons until Hover-- */
/* Hide mute and deafen buttons */
.panels_a4d4d9 > .container_b2ca13 .flex_bba380 > :not(:last-child) {
  opacity: 0% !important;
  width: 0px;
  transition: all 0.3s ease-in-out;
}
/* Reveal mute and Deafen buttons when settings button is hovered */
.panels_a4d4d9 > .container_b2ca13 .flex_bba380:hover > :not(:last-child) {
  opacity: 100% !important;
  width: 32px;
}
/* Resize and move the profile button to take up all the space it can to look clean. */
.avatarWrapper_b2ca13{
  transition: all 0.3s ease-in-out;
  width: 100%!important;
  margin-left: -10px;
  height: 53px;
  border-radius: 0!important;
}
/* Move the avatar back to the right a bit to look clean. */
.avatarWrapper_b2ca13 .avatar_b2ca13{
  margin-left: 10px;
}
```
</details>

## Preview

![image](https://i.imgur.com/iqNNL7J.gif)

### Credit
@riddim-glitch
@thecommieaxolotl

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

## 1.0.1

- Class revision

</details>
