# 💬 kakao-clone

## clone Kakaotalk using html, css

### 😛 Total basics 

### starting from 20/5/9 

### HTML

1. DOCTYPE : self contained tag (don't need to be closed)

2. meta : extra information

    charset : character encoding

    name = "author" 

    name = "description"

3. head / body 

    information & invisible to user - head 

    content & visible to user - body


    So meta is located in the head

4. Tags - Semantic / Non-Semantic

    * Semantic - has meaning

        ex) `<h1>`

    * Non-Semantic - no meaning 

        ex) `<div> , <span>`


5. ID / Class

    How Do I differentiate headers when I have multiple header tags? 

    because in CSS, we have to set this header should be red, this header should be blue. How ? 👀

    So here is when **ID and Class** concept steps ßin.

    ID is unique number. there is only one ID ! 

    Class can be used in multiple tags. 

### CSS

1. CSS has two Part - Selector / Property

`property-name: value;`

Then, How do I link h1 to my property?

```
h1 {
    property-name: value;
}
```

In this case, h1 ==> **selector**

If you want to describe ID or Class,

```
# ID 

#name {
    property-name: value;
    property-name: value;
}

# CLASS 

.name{
    property-name: value;
    property-name: value;
}
```

2. padding & margin

Clockwise 🕔

 * padding : TOP - RIGHT - BOTTOM - LEFT

 * padding : TOP-BOTTOM LEFT-RIGHT

3. border

 * border : width - style - color

 ex) border: 20px dashed red;


4. block

 : Doesn't accept anything else that's next to it

 ex)  `display: block;`
    
 * inline-block : allows others next to each other

 ex)  `display: inline-block;`

 * inline (=text): deletes every property 

 it's not a block anymore. like a text. 

 ex) `display: inline;`


5. position

 by deault, every box's position is static

 `position: static;`

 it means wherever you put this element, you will find it 

 * fixed 

 if you set position to `fixed`, it means it follows to be there even though you scroll. it stays with you 

 after setting position to `fixed`, you can set top, bottom, left, right 
 
 and put it on top of everything

 * absolute

 it finds relative parent, and then put it relatively to parent's position.

 in below case, .abs-box (which seems to be parent of abs-child) doesn't have `position: relative;` so parent is now body.

 So, abs-child box is positioned as 0 px from body's right 

 **because, body is always relative**

```css
.abs-box{
    width: 400px;
    height: 400px;
    background-color: yellow;
}
.abs-child{
    width: 100px;
    height: 100px;
    background-color: green;
    position: absolute;
    right: 0;
}   
```

```html
<body>
<div class="abs-box">
    <div class="abs-child"></div>
</div>
</body>
```



