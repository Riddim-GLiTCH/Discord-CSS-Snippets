# Compact Channels list
Minimizes the channels list to just the icons until you hover over then
**NOTE: This snippet is not optimized at all. This WILL cause some lag.**
(To the other CSS devs: Feel free to re-iterate this snippet to optimize it.)

## Installation
To install this snippet, simply copy the line bellow into your custom css file:
<details>
<summary>CSS</summary>

```css
/*Small channel list*/
.sidebar_e031be {
  transition: 0.3s ease-in-out;
  width: 55px;
}
.sidebar_e031be:has(.privateChannelsHeaderContainer_b22dc9){
  width: 65px;
}
.sidebar_e031be:has(.privateChannelsHeaderContainer_b22dc9) .privateChannelsHeaderContainer_b22dc9{
  opacity: 0;
  margin-top: -40px;
}
.sidebar_e031be:has(.privateChannelsHeaderContainer_b22dc9):not(:hover) .favoriteIcon__03348{
  display: none;
}
.sidebar_e031be .activityPanel_b73e7a .actions_d57dc4{
  opacity: 0;
}
.sidebar_e031be .activityPanel_b73e7a .gameIcon_fc710a,
.sidebar_e031be .container_debb33 .avatar_f8541f{
  scale: 1.3;
  margin-left: 3px;
}
.sidebar_e031be:has(.privateChannelsHeaderContainer_b22dc9) .activityPanel_b73e7a .gameIcon_fc710a,
.sidebar_e031be:has(.privateChannelsHeaderContainer_b22dc9) .container_debb33 .avatar_f8541f{
  scale: 1.3;
  margin-left: 8px;
}
.sidebar_e031be *{
  transition: ease-in-out 0.3s;
}
.sidebar_e031be .scroller__1f498{
  transition: 0.3s ease-in-out;
  margin-top: -100px;
}
.sidebar_e031be .containerDefault_e3b32b {
  transition: 0.3s ease-in-out;
  opacity: 0;
  margin-top: -40px;
}
.sidebar_e031be .container_bc43c1{
  transition: 0.3s ease-in-out;
  height: 0;
  opacity: 0;
  margin-top: -25px;
}
.sidebar_e031be .animatedContainer__0e828 {
  transition: 0.3s ease-in-out;
  opacity: 0!important;
}
.sidebar_e031be:not(:hover) .headerContent__6fcc7 {
  margin-left: 5px
}
.sidebar_e031be:not(:hover) .header__77c95 .headerChildren_e6a96f{
  display: none;
} 
.sidebar_e031be:not(:hover) .dots_a97068 {
  display: none;
}
.sidebar_e031be:not(:hover) .containerDefault_ae2ea4 .iconContainer__6a580 {
  margin-left: 0px
}
.sidebar_e031be:not(:hover) .containerDefault_ae2ea4 {
  margin-left: 5px;
  margin-right: 5px;
}
.sidebar_e031be:not(:hover) .header__77c95{
  background-color: var(--background-secondary);
  border-bottom: 1px solid var(--background-tertiary);
}
.sidebar_e031be:not(:hover) .name__4eb92, .sidebar_e031be:not(:hover) .nameTag__77ab2 {
  opacity: 0;
}
.sidebar_e031be .voiceUser__629a5 {
  margin-left: -30px;
}
.sidebar_e031be .containerDefault_ae2ea4:has(.statusDiv__1f955) .linkBottom__942a1{
  opacity: 0;
  margin-top: -15px;
}
.sidebar_e031be:not(:hover) .container_e1958d .actionButtons__85e3c, .sidebar_e031be:not(:hover) .container_e1958d .button_ae40a4 {
  width: 0;
  height: 0;
  opacity: 0;
}
.sidebar_e031be:not(:hover) .container_e1958d [href^="/channels/"]{
  display: none;
}
.sidebar_e031be:not(:hover) .container_e1958d .ping__838d2{
  scale: 1.3;
  margin-top: 2px;
  margin-left: 13px;
}
.sidebar_e031be:not(:hover) .channelInfo_b0882c, .sidebar_e031be:not(:hover) .children__563f2{
  display: none;
}
.sidebar_e031be .iconContainer__6a580{
  transition: 0.3s ease-in-out;
  margin-right: -2px;
}
.sidebar_e031be:hover .iconContainer__6a580{
  margin-right: 5px;
}
.sidebar_e031be:hover .scroller__1f498{
  margin-top: 0px;
}
.sidebar_e031be:hover .animatedContainer__0e828 {
  opacity: 1!important;
}
 .sidebar_e031be:hover .containerDefault_e3b32b {
  height: unset!important;
  opacity: unset!important;
  margin-top: unset;
}
.sidebar_e031be:hover .container_bc43c1{
  height: unset;
  opacity: 1;
  margin-top: 0;
}
.sidebar_e031be:hover .voiceUser__629a5 {
  margin-left: 0;
}
.sidebar_e031be:hover .containerDefault_ae2ea4:has(.statusDiv__1f955) .linkBottom__942a1{
  opacity: 1;
  margin-top: unset;
}
.sidebar_e031be:hover .activityPanel_b73e7a .actions_d57dc4{
  opacity: 1;
}
.sidebar_e031be:hover .activityPanel_b73e7a .gameIcon_fc710a,
.sidebar_e031be:hover .container_debb33 .avatar_f8541f{
  scale: unset;
  margin-left: unset;
}
.sidebar_e031be:hover{
  width: 250px!important;
}


/*Settings Icon Hotfix!!*/
.sidebar_e031be:not(:hover) .container_debb33 .flex_f18b02 {display: none}
```

</details>

## Preview
![image](https://Riddim-GLiTCH.hacked-your.tech/content/cdn/gexyALBsdjSG.gif)


### Credit
@riddim_glitch

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

## 1.1.0

- Updated snippet to account for previously missed inconsistencies and fixed a lot of issues. This snippet increased in size drastically from this (57 > 137 lines of CSS!)
- Snippet will now only be available through Github, as it exceeds the text limit for Discord Messages, Even with Nitro.

## 1.1.1 Hotfix

- Fixed an issue where the user area buttons would appear over the avatar by removing the buttons until sidebar is hovered.

## 1.1.2 Class Fix
- Updated the classes to match Discord's new ones.

</details>
