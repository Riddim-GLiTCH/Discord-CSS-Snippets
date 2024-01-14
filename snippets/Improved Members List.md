# Improved Members List
Minimizes the members list to just the members' avatars until you hover over them.

## Installation
To install this snippet, simply add the following code to your CSS file.
```css
/*Small Member list*/
.container_b2ce9c {
  transition: 0.3s ease-in-out;
  margin-right: -180px;
}
.container_b2ce9c .membersGroup__85843 {
  transition: 0.3s ease-in-out;
  height: 0px!important;
  margin-top: -25px;
}
.container_b2ce9c:hover .membersGroup__85843 {
  height: unset!important;
  margin-top: unset!important;
}
.container_b2ce9c:hover{
  margin-right: unset!important;
}
```

## Preview
![image](https://i.imgur.com/fr8kSpM.gif)

### Credit
@riddim_glitch

<details>
<summary>Changelog</summary>

## 1.0.0

- Initial release

</details>
