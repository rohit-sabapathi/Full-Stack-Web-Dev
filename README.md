This repository Contains the files, the i used to learn and perform exercise based on WEB-Development.


CSS - Notes:
    Order of Importance or Execution:
        1. Important:
                    The '!important' keyword has the highest importance while css execution. This keyword is applied to the css statement and it overrides all the other css statements if used and applies this one.
        2. Type:
                The type of css like external, inline, internal, has their own form of importance and they are ordered or executed in the below:
                    1. Inline
                    2. Internal
                    3. External
        3. Specificity:
                    The specificity is a term is used to denote the importance of the each Selector used in CSS. It determines the priority of each selector, or in which order it should be used:
                        1. #Id-Name - Id selector
                        2. element[attribute] - Attribute Selector
                        3. .Class-Name - Class selector
                        4. Element - Element selector
                        5. * - Universal Selector
        4. Position:
                    Consider the below example:
                    li {
                        color: red;
                        color: pink;
                    }
                    The color 'red' will apply first, and when the next color is read, it changes to the 'pink' color because the position matters.

    Combinators in CSS:
        There are a few types of 

    CSS - positioning:
        Css positioning is defined as the position where your css elements are placed in the Web Page.They are produced in the following types:
            1. Static Position:
                            This is the default position of the html element when it is added to the webpage.
                                ex: position: static;
            2. Relative Position:
                            This is the relative position of the webpage, where you can change the it's position for it default location to the position where it looks good on.
                                ex: position: relative;
                                    top: 30px;
                                    left: 30px;
            3. Absolute Position:
                            This position is relative to it's absolute or nearest ancestor position. Which means the it's default position changes from it's original position to the nearest ancestor's or parents's position if it has one. Else it's position is set to the webpage's left corner.
                                ex: position: absolute;
                                    top: 40px;
                                    left: 40px;
            4. Fixed Position:
                            This position is relative to the Browser's Window, means that at the load of the webpage the element will be placed at the left corner of the webpage, but when you scroll down the webpage, it moves along with the webpage.
                                ex: position: fixed;
                                    top: 50px;
                                    left: 50px;
            Note:
                z-index(property of css):
                    This is used to represent the element below or on the other elements, which means if this property's value is high enough than other element's 'z-index' value, then it stays or displays on top of that element. If it's value is lower than the other element it goes underneath the other element. i.e. the element may be hidden or partially displayed.
                        ex: z-index: -1;    <!-- Shows underneath the other elements -->
                            z-index: 0;     <!-- Shows on the other elements if they doesn't have this property -->
                            z-index: 400;   <!-- Shows on the other elements if the value of this property in the              other elements are low to this element -->