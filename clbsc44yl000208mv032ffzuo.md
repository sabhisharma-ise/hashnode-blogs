# Absolute Positioning in CSS

### 🌐 In this article, we will understand how absolute positioning works in CSS.

## **📌** Absolute Position

Consider an image that’s inside a div, so the div is colored red and has a relative position. Now our image is nested inside that div and we have given it an absolute position.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671303340439/hCkzSAsp-.png align="center")

```css
div {
	position: relative;
}

img {
	position: absolute;
	right: 30px;
}
```

Now if we change the right-coordinate property to 30px.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671303549961/-H9-41Qu8.png align="center")

The image is positioned relative to its parent (in this case, that red div). In this case, we have added a right margin of 30px between the image element and the parent div.

## **📌 Things to Remember in Absolute Position**

*   The first thing to notice in absolute positioning is that it does affect the flow of your HTML. So, unlike relative positioning where it still kept the positions of everything else the same, in absolute positioning, we are taking the element out of the flow of the document and it’s no longer considered part of the natural flow of the document.
    
*   We can move an element anywhere on the screen relative to its parent.
    
*   One more thing to remember is that the parent doesn’t always have to be a body. It can also be the closest parent that has a relative layout.
    

(Source: Angela Yu's **The Complete 2023 Web Development Bootcamp** [**https://www.udemy.com/course/the-complete-web-development-bootcamp/**](https://www.udemy.com/course/the-complete-web-development-bootcamp/))