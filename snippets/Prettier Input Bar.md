# Prettier Input Bar
Makes the Message input bar prettier by hiding the overload of buttons behind a hamburger menu, which is easily expanded by hovering over it.

## Installation
To install this snippet, simply copy the CSS bellow into your custom CSS file:
<details>
<summary>CSS</summary>

```css
[class^=channelTextArea_] [class^=buttons_]::before,
[class^=channelTextArea_] [class^=buttons_]::after /* Adds a new button to the text area */ {
  content: "≡";
  font-size: 2rem;
  scale: 1;
  color: var(--interactive-normal);
  display: flex;
  align-items: center;
  position: absolute;
  right: 100%;
  height: 100%;
  transition: scale 0.3s 0.1s ease-in-out;
}
[class^=channelTextArea_] [class^=buttons_]::after /* Makes the 'after' field invisible. There is an 'after' to prevent jitteriness. */ {
  color: transparent;
}
[class^=channelTextArea_] [class^=buttons_] /* Hide all buttons except for the hover button */ {
  transition: all ease-in-out 0.3s;
  translate: calc(100% - 8px);
  padding-bottom: 5px;
  padding-left: 20px;
}
[class^=channelTextArea_] [class^=buttons_] [class^=button_] /* Adjust the width and visibility of the buttons for a smoother transition */ {
  transition: all ease-in-out 0.3s;
  width: 0;
  opacity: 0;
}
[class^=channelTextArea_] [class^=buttons_]:hover /* Reveal all buttons on hover */ {
  translate: 0%;
  padding-left: 0px !important;
}
[class^=channelTextArea_] [class^=buttons_]:hover [class^=button_] /* Adjust the width and visibility of the buttons to make them actually visible */ {
  transition: all ease-in-out 0.5s;
  width: unset;
  opacity: 1;
}
[class^=channelTextArea_] [class^=buttons_]:hover::before /* Hide the hover button on hover */ {
  margin-right: 8px;
  scale: 0 1;
}
```
</details>

## Preview
![Vesktop_7lWYNSnmEM](https://github.com/Riddim-GLiTCH/Discord-CSS-Snippets/assets/87764384/b1088974-02ac-434a-a2e6-6f044678808b)


### Credit
@riddim-glitch

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

</details>
