# Improved User Area
Small improvements to the User Area. Displays your screen name, User Name and Status message all at once. Adds an @ to the username (Because apparently Discord doesn't know how usernames work 👍 )
Also hides the mute and deafen buttons until you hover over the settings button. (This is a modified version of the Hide User Buttons until Hover snippet by [@TheCommieAxolotl](https://github.com/TheCommieAxolotl))


## Installation
<details>
<summary>CSS</summary>

```css
.container_ca50b9 .hovered__243e5, .hoverRoll__041cb.forceHover__71322:not(.disabled__89e5c) .default_cae228{
  opacity: 1!important;
  transform: none;
}
.container_ca50b9 .hovered__243e5::before{
  content: "@";
}
.default_cae228{
  margin-top: 15px;
}
.panels__58331 > .container_ca50b9 .flex_f5fbb7 > :not(:last-child) {
  opacity: 0% !important;
  width: 0px;
  transition: all 0.3s ease-in-out;
}
.panels__58331 > .container_ca50b9 .flex_f5fbb7:hover > :not(:last-child) {
  opacity: 100% !important;
  width: 32px;
}
.avatarWrapper_ba5175{
  transition: all 0.3s ease-in-out;
  width: 100%!important;
  margin-left: -10px;
  height: 53px;
  border-radius: 0!important;
}
.avatarWrapper_ba5175 .avatar_f8541f{
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

</details>
