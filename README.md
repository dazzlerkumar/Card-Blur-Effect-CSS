# Card Blur Effect CSS
On hover over a card the remaining cards will go blurred. 
___

![](/assets/preview.gif "Card Blur Effect GIF")

### HTML Part
###### Refer to [index.html](/index.html) file

We have a division with `id="featureImgs"` which contains all the image boxes, all positioned center using Bootstrap 4 and we have a class for image boxes `class="featureImg"`.
Using these two selectors, we're gonna make the **blur effect on hover**. 

### CSS Part
###### Refer to [styles.css](/styles.css) file

**Step 1. Blur all the cards on hover of the container**

    #featureImgs:hover .featureImg{
        filter: blur(10px);
        transform: scale(0.9);
        opacity: 0.5;
    }

Here, were are targeting the children class of the contrainer `featureImgs`.
On hovering the cursor, rest of the cards will be blurred and scaled to 0.9 times of the actual size.


**Step 2. Bringing the card in focus on hover of the mouse**

    #featureImgs .featureImg:hover{
    filter: blur(0px);
    transform: scale(1.05);
    opacity: 1;
    }

Here, were are targeting the children class of the contrainer `featureImgs` on hovering over one of them.
On hovering the cursor, the cards will be focused and scaled to 1.05 times of the actual size.
___

*You can add more effects such giving shadows to the focused card on hover and et cetera.*



