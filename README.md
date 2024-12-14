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
                            z-index: 400;   <!-- Shows on the other elements if the value of this property in the other elements are low to this element -->

    CSS - Display property:
        1. Block:
            This is the default display value, where it takes the full width of the webpage and height as the content's height, it makes only one element to appear in a single line in a webpage.
        2. Inline:
            This makes the element to be appeared in the same line in the webpage. The size of these elements like height and width, because they will have the size of their content.
        3. Inline-Block:
            This takes both the functions of Block and Inline, you make more elements to appear in a single line and can change the width and height of the content.
        4. None:
            This value of the display property makes the element to be hidden or removed from the webpage.

    CSS - Float Property:
        This Property is used to make the text or element wrap up with other element of the webpage.
            1. Left:
                This value of the float property, makes the element it is applied on to move to the left side, by pushing other element it is wrapped to the right side.
            2. Right:
                This value of the float property, makes the element it is applied on to move to the right side, by pushing other element it is wrapped to the left side.
        Note:
            The above property can be undone, which means if other elements are wrapped around the element which have float property and you don't want to have it like that, you can remove the element around the float element, by giving those element with clear property:
                1. Clear(property):   Value => left, right, both.
                    This property will remove the wrapping around the float element and if the float element has 'left' value then this should also have 'left' value to undo the same. It goes vice versa for the 'right' value also.If the element is wrapped with both the float values then use 'both' value to undo the wrapping with those elements.

    CSS - Responsive Design:
        This can be implemented in 4 ways:
            1. Media Query:
                This method is used to design the webpage which width is below or equal to the mentioned value.
                    ex: @media (max-width: 500px){
                        /*CSS code for web design which is below to equal to 500px width */
                    }
            2. CSS Grid:
                This method is used to group a number of elements in the webpage in a table form for arranging them in a rows and columns to make them look good and responsive. This method works for 2D layouts like a table.
            3. Flex Box:
                This method is used to design 1D layouts like row , column etc.
            4. Bootstrap Framework:
                This is an external css document which contains predefined codes which can you used in out website.

    Media Query:
        This responsive design is used to override the other css properties, if the window size increases or decreases according to the rule mentioned in the stylesheet. For example read the following:
            1. To display the content of the webpage when the window is smaller, the 'max-width' property is used.
                This property will apply the styles mentioned in it, when the max-width of the webpage is lesser or equal to the value of the mentioned in it.
                    ex: @media (max-width: value){           /* This line is called BreakPoint */
                        /* Styles that should be applied when the above breakpoint is True */
                    }
            2. To display the content of the webpage when the window is bigger, the 'min-width' property is used.
                This property will apply the styles mentioned in it, when the min-width of the webpage is larger or equal to the value of the mentioned in it.
                    ex: @media (min-width: value){
                        /* Styles that should be applied when the above breakpoint is True */
                    }
            3. To display the content of the webpage within a range of the window size, you can combine both the properties to do the mentioned and vice versa. This will only apply the styles in the media query, when the window is equal to or in the range of the mentioned BreakPoint.
                ex: @media (min-width: value) and (max-width: value){
                    /* Styles will be applied if only the webpage is between the above BreakPoint */
                }
                ex: @media (max-width: value) and (min-width: value){
                    /* Styles will be applied if only the webpage is not between the above BreakPoint */
                }

