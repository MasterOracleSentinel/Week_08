CSS selectors and inheritance are the key concepts required to make more specific and elegant styles as you begin working in CSS. 

In CSS, you style HTML elements . These selectors can be either an HTML tag, a class name, or an ID. You can also combine these selectors to target more specific HTML elements.

Why do selectors matter? 

You may think, “Ok, that's cool, but why does this matter? Why not just give everything a class name and be done with it?”

The reason is there are different “layers” of CSS, which comes down to a very common principle in programming called “inheritance.” Much like a human child inherits traits from their parents, such as their eye or hair color, elements of code inherit traits from their parent elements. 

For example, suppose you write the following HTML code: 


![image](https://user-images.githubusercontent.com/105542222/213896505-62857381-4e6a-490a-a7b9-3228a2b60027.png)

Selectors impact parent-child elements 

As you can see, there are two div elements, where one has the class "parent" and the other has the class "child." If you target the parent class in CSS and give it a style, the child elements will also have the same style, because they have inherited it from their parent elements. 


![image](https://user-images.githubusercontent.com/105542222/213896512-d7fe90e6-beee-4553-bdc6-a00863e312a9.png)

However, just as human children are not carbon copies of their parents, sometimes child elements in code have their own particular styles. When a child element has a specific style, it takes priority over the parent element's style. 


![image](https://user-images.githubusercontent.com/105542222/213896519-16a6f15d-0c8e-4520-a7af-c60557e5ead2.png)

In other words, the more specific the targeting of a particular element, the more control you have over its styling.  

To target the same element with separate selectors, you can use different punctuations. To target a simple tag, you can simply write the tag name. To target a class, put a period followed by the class name (.class-name). For an ID, put a hash sign, followed by the ID name (#id-name). A similar idea of inheritance is at play here, as not all selectors are equal. A tag selector is the lowest priority, then a class name, and then an ID. So, if you have three HTML elements of:


![image](https://user-images.githubusercontent.com/105542222/213896524-0e659d7d-6a13-440d-83b6-48591f7471a6.png)

Now, if you want to style the second “Hello” differently, you'll need to target it by its class name. What do you think will happen?


![image](https://user-images.githubusercontent.com/105542222/213896528-fd24a43e-fb5b-42a9-b98b-c2fcef154769.png)

If you guessed that the element with the class name "greeting" will turn green and the other elements will stay orange, you’re correct. But you may be wondering how that can be when there are two h1 elements with the same name. It’s because one of them is a class name and one of them is an ID name. Since you only targeted the element with the class name using ".greeting," that’s the only one that changed color. 


To target the last element, which has a div ID of “greeting,” use a pound sign. 

![image](https://user-images.githubusercontent.com/105542222/213896536-c8027e1e-20ad-4da2-864b-561fe8ca9461.png)

This will turn the last element blue

![image](https://user-images.githubusercontent.com/105542222/213896543-3b8d03d9-049c-4ab2-914f-48c6aa8da3bb.png)

Using this cascade and its different targeting abilities with parent/children elements as well as using class and ID selectors will be an ongoing learning process, which will prove very useful in your journey as a developer.


