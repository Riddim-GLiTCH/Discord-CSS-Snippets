# Improved Links
Modifies the appearance of plain links to look more like a channel/user mention.
Also optionally unhides the masked links from Discord's recently added markdown feature.

## Installation
To install this snippet, simply copy the text below into your custom css file:

<details>
<summary>CSS</summary>

```css
[class^=message_] [class^=contents_] [class^=anchor_], [class^=message_] [class^=repliedMessage_] [class^=anchor_], [class^=message_] [class^=modal] [class^=anchor_], [class^=message_] [class^=topic_] [class^=anchor_], [class^=focusLock] [class^=contents_] [class^=anchor_], [class^=focusLock] [class^=repliedMessage_] [class^=anchor_], [class^=focusLock] [class^=modal] [class^=anchor_], [class^=focusLock] [class^=topic_] [class^=anchor_], [class^=title] [class^=contents_] [class^=anchor_], [class^=title] [class^=repliedMessage_] [class^=anchor_], [class^=title] [class^=modal] [class^=anchor_], [class^=title] [class^=topic_] [class^=anchor_] {
  transition: background-color 50ms ease-out, color 50ms ease-out;
  color: var(--mention-foreground);
  background-color: var(--mention-background);
  padding: 1px 2px;
  border-radius: 3px;
  border-bottom: 1px solid var(--brand-700);
}
[class^=message_] [class^=contents_] [class^=anchor_]::before, [class^=message_] [class^=repliedMessage_] [class^=anchor_]::before, [class^=message_] [class^=modal] [class^=anchor_]::before, [class^=message_] [class^=topic_] [class^=anchor_]::before, [class^=focusLock] [class^=contents_] [class^=anchor_]::before, [class^=focusLock] [class^=repliedMessage_] [class^=anchor_]::before, [class^=focusLock] [class^=modal] [class^=anchor_]::before, [class^=focusLock] [class^=topic_] [class^=anchor_]::before, [class^=title] [class^=contents_] [class^=anchor_]::before, [class^=title] [class^=repliedMessage_] [class^=anchor_]::before, [class^=title] [class^=modal] [class^=anchor_]::before, [class^=title] [class^=topic_] [class^=anchor_]::before {
  content: "🔗";
  margin-right: 2px;
  filter: saturate(0%);
  font-size: small;
}
[class^=message_] [class^=contents_] [class^=anchor_]:hover, [class^=message_] [class^=repliedMessage_] [class^=anchor_]:hover, [class^=message_] [class^=modal] [class^=anchor_]:hover, [class^=message_] [class^=topic_] [class^=anchor_]:hover, [class^=focusLock] [class^=contents_] [class^=anchor_]:hover, [class^=focusLock] [class^=repliedMessage_] [class^=anchor_]:hover, [class^=focusLock] [class^=modal] [class^=anchor_]:hover, [class^=focusLock] [class^=topic_] [class^=anchor_]:hover, [class^=title] [class^=contents_] [class^=anchor_]:hover, [class^=title] [class^=repliedMessage_] [class^=anchor_]:hover, [class^=title] [class^=modal] [class^=anchor_]:hover, [class^=title] [class^=topic_] [class^=anchor_]:hover {
  background-color: var(--brand-experiment);
}
```
</details>


Optionally add this extra snippet to unhide masked links:
<details>
<summary>CSS</summary>

```css
.anchor_c8ddc0[title$=")"]:after {
  font-size: 0.7rem;
  content: " (" attr(href) ")";
  filter: grayscale(0.5);
}
```

</details>

## Preview
![Preview](https://imgur.com/FOqhVCI.png)

### Credit
@Riddim_GLiTCH

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

</details>
