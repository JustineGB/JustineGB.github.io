---
layout: post
title:      "Flexible Box Layouts"
date:       2019-10-10 11:36:08 -0400
permalink:  flexible_box_layouts
---


Flexible Box Layout (CSS3 FlexBox) allows you to create flexible and responsive webpages without having to resort to complicated positioning and floats. FlexBox was first introduced back in 2009, but it has evolved a lot since then. 

If you need to have both rows and columns shown in your application view, I would recommend using Grid instead of FlexBox. If you have a list of items to display within a container or you have a few text boxes you want to display side-by-side on a page, I would recommend using FlexBox. 

To get started using FlexBox, you need a parent container and within that parent container, you will nest the child boxes/items. The parent is control, for better or worse. 

![](https://media.giphy.com/media/DbbHysLg3LCF2/giphy.gif)

First, add “display: flex” to you parent container. You can add a number of features to the parent container such as flex direction, flex wrap, flex flow, justify content, align items, and align content. 

The flex direction will allow you to determine if you want to place your items into a row (side-by-side) or a column (up and down). If you have a large list and you want it spaced out in a row format but over multiple rows, you will use flex wrap. You can even specify column-reverse if you want to list your items in a column from bottom-to-top (you can do the same with wrap-reverse). Justify Content allows you to align the items in the center, left, or right. You can add align-content stretch to stretch the flex lines to take up the remaining space (this is actually the default value). 

For the child or item elements nested within the container you can add a number of features such as order, flex grow flex shrink, flex basis, and align self. Flex basis is interesting to use as it will allow you to size all of your items/child boxes equally within the container or you can leave it set to auto and it will allow the item/box to be as big as it needs to be to fit the text within. For shrink and grow, you can set specific items to grow or shrink in comparison to the other items within the container.

Overall, FlexBox is a great feature to use because it is supported in almost all web browsers, it is easy to use, and it allows for responsive and flexible webpages. You can easily space items and center items with just a few lines of code. Pretty neat! 

![](https://media.giphy.com/media/l0Nwvo3slpo6nS0PC/giphy.gif)


