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
.sidebar_a4d4d9 {
  transition: 0.3s ease-in-out;
  width: 55px;
}
.sidebar_a4d4d9:has(.privateChannelsHeaderContainer_c47fa9){
  width: 65px;
}
.sidebar_a4d4d9:has(.privateChannelsHeaderContainer_c47fa9) .privateChannelsHeaderContainer_c47fa9{
  opacity: 0;
  margin-top: -40px;
}
.sidebar_a4d4d9:has(.privateChannelsHeaderContainer_c47fa9):not(:hover) .favoriteIcon_c91bad{
  display: none;
}
.sidebar_a4d4d9 .activityPanel_a4d4d9 .actions_bf1a22{
  opacity: 0;
}
.sidebar_a4d4d9 .activityPanel_a4d4d9 .gameIcon_f394e5,
.sidebar_a4d4d9 .container_b2ca13 .avatar_b2ca13{
  scale: 1.3;
  margin-left: 3px;
}
.sidebar_a4d4d9:has(.privateChannelsHeaderContainer_c47fa9) .activityPanel_a4d4d9 .gameIcon_f394e5,
.sidebar_a4d4d9:has(.privateChannelsHeaderContainer_c47fa9) .container_b2ca13 .avatar_b2ca13{
  scale: 1.3;
  margin-left: 8px;
}
.sidebar_a4d4d9 *{
  transition: ease-in-out 0.3s;
}
.sidebar_a4d4d9 .scroller_c43953{
  transition: 0.3s ease-in-out;
  margin-top: -100px;
}
.sidebar_a4d4d9 .containerDefault_a08117 {
  transition: 0.3s ease-in-out;
  opacity: 0;
  margin-top: -40px;
}
.sidebar_a4d4d9 .container_c75f85{
  transition: 0.3s ease-in-out;
  height: 0;
  opacity: 0;
  margin-top: -25px;
}
.sidebar_a4d4d9 .animatedContainer_fd6364 {
  transition: 0.3s ease-in-out;
  opacity: 0!important;
}
.sidebar_a4d4d9:not(:hover) .headerContent_fd6364 {
  margin-left: 5px
}
.sidebar_a4d4d9:not(:hover) .header_fd6364 .headerChildren_fd6364{
  display: none;
} 
.sidebar_a4d4d9:not(:hover) .dots_ce0450 {
  display: none;
}
.sidebar_a4d4d9:not(:hover) .containerDefault_f6f816 .iconContainer_d8bfb3 {
  margin-left: 0px
}
.sidebar_a4d4d9:not(:hover) .containerDefault_f6f816 {
  margin-left: 5px;
  margin-right: 5px;
}
.sidebar_a4d4d9:not(:hover) .header_fd6364{
  background-color: var(--background-secondary);
  border-bottom: 1px solid var(--background-tertiary);
}
.sidebar_a4d4d9:not(:hover) .name_d8bfb3, .sidebar_a4d4d9:not(:hover) .nameTag_b2ca13 {
  opacity: 0;
}
.sidebar_a4d4d9 .voiceUser_cdc675 {
  margin-left: -30px;
}
.sidebar_a4d4d9 .containerDefault_f6f816:has(.statusDiv_e66732) .linkBottom_d8bfb3{
  opacity: 0;
  margin-top: -15px;
}
.sidebar_a4d4d9:not(:hover) .container_adcaac .actionButtons_adcaac, .sidebar_a4d4d9:not(:hover) .container_adcaac .button_f67531 {
  width: 0;
  height: 0;
  opacity: 0;
}
.sidebar_a4d4d9:not(:hover) .container_adcaac [href^="/channels/"]{
  display: none;
}
.sidebar_a4d4d9:not(:hover) .container_adcaac .ping_c0cb95{
  scale: 1.3;
  margin-top: 2px;
  margin-left: 13px;
}
.sidebar_a4d4d9:not(:hover) .channelInfo_f6f816, .sidebar_a4d4d9:not(:hover) .children_d8bfb3{
  display: none;
}
.sidebar_a4d4d9 .iconContainer_d8bfb3{
  transition: 0.3s ease-in-out;
  margin-right: -2px;
}
.sidebar_a4d4d9:hover .iconContainer_d8bfb3{
  margin-right: 5px;
}
.sidebar_a4d4d9:hover .scroller_c43953{
  margin-top: 0px;
}
.sidebar_a4d4d9:hover .animatedContainer_fd6364 {
  opacity: 1!important;
}
 .sidebar_a4d4d9:hover .containerDefault_a08117 {
  height: unset!important;
  opacity: unset!important;
  margin-top: unset;
}
.sidebar_a4d4d9:hover .container_c75f85{
  height: unset;
  opacity: 1;
  margin-top: 0;
}
.sidebar_a4d4d9:hover .voiceUser_cdc675 {
  margin-left: 0;
}
.sidebar_a4d4d9:hover .containerDefault_f6f816:has(.statusDiv_e66732) .linkBottom_d8bfb3{
  opacity: 1;
  margin-top: unset;
}
.sidebar_a4d4d9:hover .activityPanel_a4d4d9 .actions_bf1a22{
  opacity: 1;
}
.sidebar_a4d4d9:hover .activityPanel_a4d4d9 .gameIcon_f394e5,
.sidebar_a4d4d9:hover .container_b2ca13 .avatar_b2ca13{
  scale: unset;
  margin-left: unset;
}
.sidebar_a4d4d9:hover{
  width: 250px!important;
}


/*Settings Icon Hotfix!!*/
.sidebar_a4d4d9:not(:hover) .container_b2ca13 .flex_bba380 {display: none}
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
