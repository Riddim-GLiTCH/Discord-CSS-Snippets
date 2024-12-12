# Right Side Attach Button
Move That Attachment Button to the Right of your Message Input Box!
> [!WARNING]
> Not compatible with [Prettier Input Bar](https://github.com/Riddim-GLiTCH/Discord-CSS-Snippets/blob/main/snippets/Prettier%20Input%20Bar.md).</br>
> May be incompatible with certain plugins.</br>

Tested with most **Vanilla** use cases.</br>
Works with Send Button Enabled.<br>
<details>
<summary>Currently known issues:</summary>

- Will Break when a certain amount of linebreaks are passed while an attachment is present. 
  - I have an idea on how to fix this, but its probably gonna be hella janky and I don't really feel like testing that theory right now cuz its a very niche scenario and it can easily be dismissed in the rare case it does happen.
- Hover does not actually make the button glow.
  - I'll either find a workaround to `drop-shadow()` or just scrap the glow effect. Growing the button should already be enough for enhanced responsiveness.

</details>


## Installation
To install this snippet, simply copy the CSS bellow into your custom css file:</br>
<details>
<summary>CSS</summary>

```css
/* Right-Side Attach Button */
.channelTextArea_a7d72e {
  .emojiButton_bdf0de  {
    margin-right: 45px
  }
  .attachWrapper_f298d4 {
    position:fixed;
    transition: all ease 0.15s;
    right: 0;
    z-index: 20; /* The Emoji Button Likes to Make the Attach Button impossible to click by being over it.
                    This makes it not do that. Might be a Z-index or two too many though. */
    &:hover {
      scale: 1.3;
      translate: 2px;
      filter: drop-shadow(0 0 2px currentColor);
    }
  }
  :has(.sendIcon_a06035) { /* ONLY MOVE THE BUTTON BY 50PX IF THE SEND BUTTON IS PRESENT */
     /* There is probably a more optimal way to do this tbh. But this works so its fine. */
    .attachWrapper_f298d4 {
      position: fixed;
      transition: all ease 0.15s;
      right: 50px;
      z-index: 20; /* The Emoji Button Likes to Make the Attach Button impossible to click by being over it.
                      This makes it not do that. Might be a Z-index or two too many though. */
      &:hover {
        scale: 1.3;
        translate: 2px;
        filter: drop-shadow(0 0 2px currentColor);
      }
    }
  }
}
```

</details>

## Previews
### What it should look like:
![DiscordDevelopment_v4zTdYyABj](https://github.com/user-attachments/assets/d019697d-797a-4959-937e-907268b4ab05)</br>
### Example Use Case - An IRC Styled theme:
![DiscordDevelopment_PvOhV3xMyR](https://github.com/user-attachments/assets/890fe1ac-b728-4f21-8f81-ea129fe44afc)


### Credit
@Riddim_GLiTCH

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

</details>
