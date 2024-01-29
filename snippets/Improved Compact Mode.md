# Improved Compact Mode
Improves the appearance of Compact mode, To make it look more like a proper chat app.
Due to the amount of things discord keeps adding to the message header, and the lack of a semicolon to indicate that a user is speaking, I felt the need to clean some stuff up. So here it is, my attempt at fixing compact mode.

**COMPATIBILITY NOTICE**
Snippet may break on some themes. However, it should be noted that most themes are designed with COZY mode in mind. I will NOT be adding compatibility for specific themes. If the snippet breaks a theme, it is not my problem.


## Installation
To install this snippet, simply copy the CSS bellow into your custom css file:
<details>
<summary>CSS</summary>

```css
/* Add a colon behind the username */
[class*="compact_"] [class^="headerText_"] [class^="separator_"] {
    color: var(--text-primary);
    position: unset;
    opacity: unset;
    display: initial;
    font-size: larger;
    margin-left: .5px;
  }
/* Remove the reply icon for a cleaner look. */
[class*="compact_"] [class^=replyBadge_] {
  display: none;
}

/* Fix replies. (now actually fixes them) */
[class*="compact_"] [class^="repliedMessage_"] [class^="username_"]:after{
  color: var(--text-normal)!important;
  content: ":";
  font-size: larger;
 }

/* Move the New Member icon and the Role Badge to before the username (untested if both are present. Will Likely break!) */
[class*="compact_"] [class^="headerText_"]:has([class^=roleIcon_], [class^=newMemberBadge_]) {
	margin-left: 23px;
} 
  
[class*="compact_"] [class^="headerText_"] [class^=roleIcon_], [class^="headerText_"] [class^=newMemberBadge_] {
    position: absolute;
    left: 87.5px;
  }
/* Move the Silent Message icon to before the timestamp. (untested with anything other than 12h AM/PM standard past noon.) */
body:has([class^=messagesWrapper_] [class*="compact_"]) [class^=message_] [class^=badge_]:has(svg path[d^="M19 11.5a.5.5 0 0 0-.5-.5h-2.33a2.5 2.5 0 0 1-2.5-2.5v-1a3"]) {
  position: absolute;
  left: 7px;
  top: 4.5px;
}
```
</details>

Then change the following Settings:
>Appearance
>>Compact Mode: ON<br>
>>Avatars in Compact Mode: ON

## Preview
![image](https://github.com/Riddim-GLiTCH/Discord-CSS-Snippets/assets/87764384/89c31375-d0a6-42af-9955-fdea2c5b5058)
### Credit
@Riddim_GLiTCH

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

## 2.0.0

- Rewrite to work with new classes
- Minor fixes

## 3.0.0

- Added compact mode detection; changes should now only apply when Compact mode is enabled. Nothing will happen in Cozy mode
- Removed the hiding of the timestamps as it broke the edited message notice. Timestamps are also a requirement now for the silent message icon to appear correctly.
- Moved new member badge and role icons to before the username. Astatically more pleasing. (Note, Untested if both are present. I expect the icons to just overlap. However, due to the rarity of this event, I will NOT be adding checks for this. Too much hassle for a problem that is unlikely to ever occur.)
- Moved Silent Message icon from after the separator to before the timestamp. "name::bell: message" doesn't make a lot of sense, and putting it there instead made the most amount of sense to me.

</details>
