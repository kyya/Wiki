---
description: Markdown Cheat Sheet For MkDocs - How to Embed Gists, YouTube Videos, Lucid Charts
---

# Embedding External Sources

## Gists Embedding

Example:

```html
<script src="https://gist.github.com/fire1ce/bc8d0ab9e1aeb4c83b46a22df7846625.js"></script>
```

__Result:__
<script src="https://gist.github.com/fire1ce/bc8d0ab9e1aeb4c83b46a22df7846625.js"></script>

## Embedding YouTube Videos

Default: Width=480 Hight=270

```markdown
[!embed](https://www.youtube.com/watch?v=vq2jYFZVMDA)
```

With Costume width=1200

```markdown
[!embed?max_width=1200](https://www.youtube.com/watch?v=vq2jYFZVMDA)  
```

With Costume width=300, height=200

```markdown
[!embed?max_width=300&max_height=200](https://www.youtube.com/watch?v=vq2jYFZVMDA)
```

__Will Render to:__

Default: Width=480 Hight=270  
[!embed](https://www.youtube.com/watch?v=vq2jYFZVMDA)

With Costume width=1200  
[!embed?max_width=1200](https://www.youtube.com/watch?v=vq2jYFZVMDA)  

With Costume width=300, height=200  
[!embed?max_width=300&max_height=200](https://www.youtube.com/watch?v=vq2jYFZVMDA)

## Lucid Charts Embedding

[lucidchart.com](https://www.lucidchart.com/ "lucidchart.com")

open the Lucid chart and select the share -> embed menu item. click the `activate embed code` and copy and past the HTML.

![lucid](../assets/images/MarkdownCheatSheet/lucid_char_html.png)

> :bulb: its recommended to change the width to 100% and remove the margin and relative setting under style

```html
<div style="width: 100%; height: 520px;">  
<iframe allowfullscreen frameborder="0"
style="width:100%; height:520px"
src="https://www.lucidchart.com/documents/embeddedchart/ee9393c4-427d-4390-97da-1d0a42b5823e"
id="n8kd1lbHuhin">
</iframe>
</div>
```

<div style="width: 100%; height: 600px;">
<iframe allowfullscreen frameborder="0" style="width:100%; height:600px" src="https://www.lucidchart.com/documents/embeddedchart/ee9393c4-427d-4390-97da-1d0a42b5823e"
id="n8kd1lbHuhin"></iframe>
</div>
