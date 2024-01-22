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
.sidebar_ded4b5 {
    transition: 0.3s ease-in-out;
    width: 55px;
  }
  .sidebar_ded4b5:has(.privateChannelsHeaderContainer_ddcec6){
    width: 65px;
  }
  .sidebar_ded4b5:has(.privateChannelsHeaderContainer_ddcec6) .privateChannelsHeaderContainer_ddcec6{
    opacity: 0;
    margin-top: -40px;
  }
  .sidebar_ded4b5:has(.privateChannelsHeaderContainer_ddcec6):not(:hover) .favoriteIcon_b001ac{
    display: none;
  }
  .sidebar_ded4b5 .activityPanel__22355 .actions__9256d{
    opacity: 0;
  }
  .sidebar_ded4b5 .activityPanel__22355 .gameIcon__90c32,
  .sidebar_ded4b5 .container_ca50b9 .avatar_f8541f{
    scale: 1.3;
    margin-left: 3px;
  }
  .sidebar_ded4b5:has(.privateChannelsHeaderContainer_ddcec6) .activityPanel__22355 .gameIcon__90c32,
  .sidebar_ded4b5:has(.privateChannelsHeaderContainer_ddcec6) .container_ca50b9 .avatar_f8541f{
    scale: 1.3;
    margin-left: 8px;
  }
  .sidebar_ded4b5 *{
    transition: ease-in-out 0.3s;
  }
  .sidebar_ded4b5 .scroller_f0f183{
    transition: 0.3s ease-in-out;
    margin-top: -100px;
  }
  .sidebar_ded4b5 .containerDefault__23a29 {
    transition: 0.3s ease-in-out;
    opacity: 0;
    margin-top: -40px;
  }
  .sidebar_ded4b5 .container__4f639{
    transition: 0.3s ease-in-out;
    height: 0;
    opacity: 0;
    margin-top: -25px;
  }
  .sidebar_ded4b5 .animatedContainer__341f6 {
    transition: 0.3s ease-in-out;
    opacity: 0!important;
  }
  .sidebar_ded4b5:not(:hover) .headerContent_ee8727 {
    margin-left: 5px
  }
  .sidebar_ded4b5:not(:hover) .header__104ca .headerChildren__7cd0b{
    display: none;
  } 
  .sidebar_ded4b5:not(:hover) .dots_a97068 {
    display: none;
  }
  .sidebar_ded4b5:not(:hover) .containerDefault__3187b .iconContainer__3f9b0 {
    margin-left: 0px
  }
  .sidebar_ded4b5:not(:hover) .containerDefault__3187b {
    margin-left: 5px;
    margin-right: 5px;
  }
  .sidebar_ded4b5:not(:hover) .header__104ca{
    background-color: var(--background-secondary);
    border-bottom: 1px solid var(--background-tertiary);
  }
  .sidebar_ded4b5:not(:hover) .name__8d1ec, .sidebar_ded4b5:not(:hover) .nameTag__0e320 {
    opacity: 0;
  }
  .sidebar_ded4b5 .voiceUser__0470a {
    margin-left: -30px;
  }
  .sidebar_ded4b5 .containerDefault__3187b:has(.statusDiv_a4cf67) .linkBottom_bac113{
    opacity: 0;
    margin-top: -15px;
  }
  .sidebar_ded4b5:not(:hover) .container_d667ff .actionButtons_b58cbb, .sidebar_ded4b5:not(:hover) .container_d667ff .button__4f306 {
    width: 0;
    height: 0;
    opacity: 0;
  }
  .sidebar_ded4b5:not(:hover) .container_d667ff [href^="/channels/"]{
    display: none;
  }
  .sidebar_ded4b5:not(:hover) .container_d667ff .ping__47992{
    scale: 1.3;
    margin-top: 2px;
    margin-left: 13px;
  }
  .sidebar_ded4b5:not(:hover) .channelInfo_b7ab2e, .sidebar_ded4b5:not(:hover) .children_a486f8{
    display: none;
  }
  .sidebar_ded4b5 .iconContainer__3f9b0{
    transition: 0.3s ease-in-out;
    margin-right: -2px;
  }
  .sidebar_ded4b5:hover .iconContainer__3f9b0{
    margin-right: 5px;
  }
  .sidebar_ded4b5:hover .scroller_f0f183{
    margin-top: 0px;
  }
  .sidebar_ded4b5:hover .animatedContainer__341f6 {
    opacity: 1!important;
  }
   .sidebar_ded4b5:hover .containerDefault__23a29 {
    height: unset!important;
    opacity: unset!important;
    margin-top: unset;
  }
  .sidebar_ded4b5:hover .container__4f639{
    height: unset;
    opacity: 1;
    margin-top: 0;
  }
  .sidebar_ded4b5:hover .voiceUser__0470a {
    margin-left: 0;
  }
  .sidebar_ded4b5:hover .containerDefault__3187b:has(.statusDiv_a4cf67) .linkBottom_bac113{
    opacity: 1;
    margin-top: unset;
  }
  .sidebar_ded4b5:hover .activityPanel__22355 .actions__9256d{
    opacity: 1;
  }
  .sidebar_ded4b5:hover .activityPanel__22355 .gameIcon__90c32,
  .sidebar_ded4b5:hover .container_ca50b9 .avatar_f8541f{
    scale: unset;
    margin-left: unset;
  }
  .sidebar_ded4b5:hover{
    width: 250px!important;
  }

/* Settings Icon Hotfix!!!*/
.sidebar_ded4b5:not(:hover) .container_ca50b9 .flex_f5fbb7 {display: none}
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


</details>
