# Static and Relative Positioning in CSS

### 🌐 In this article, we will understand how static & relative positioning works in CSS.

## **📌** Static Position

By default, the position property for all HTML elements in CSS is set to static. This means that if you don't specify any other position value or if the position property is not declared explicitly, it'll be static.

## **📌** Relative Position

What this allows us to do, is to position the element that we select, relative to how it would have been positioned, had it been static. But just writing this CSS rule alone will not change anything.

To modify the position, you'll need to apply the top, bottom, right, and left properties mentioned earlier and in that way specify where and how much you want to move the element.

Say we have a normal flow element (Normal Flow, or Flow Layout, is the way that Block and Inline elements are displayed on a page before any changes are made to their layout), bacon image at the bottom.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671178184424/QB7Rc8aZl.png align="center")

If we apply relative positioning to this image, let’s see what happens.

```css
img {
	position: relative;
	left: 30px;
}
```

Then, it will be pushed 30px from the left of the previous position, this is how the image will end up positioned.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671178171799/ssFHeaamA.png align="center")

In contrast, if we use top: 20px, this will move the element toward the bottom of the element's parent container. Using bottom: 20px will push the element toward the top of the element's parent container, and so on.

## **📌 Things to Remember in Relative Position**

*   When we move an element, that has a relative position, it doesn’t affect the position of anything else on the screen.
    
*   When we change the coordinate properties, for example, in the example above, we are saying make the left coordinate property of this relative position 20px. What that means is that we are taking the left of where that image used to be and we are giving it a 20px margin from the left of our current image.
    

(Source: Angela Yu's **The Complete 2023 Web Development Bootcamp** [https://www.udemy.com/course/the-complete-web-development-bootcamp/](https://www.udemy.com/course/the-complete-web-development-bootcamp/))