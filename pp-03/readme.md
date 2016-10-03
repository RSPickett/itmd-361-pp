## ITMD 361, Production Problem 3: Relative Units in CSS

For this production problem, you will be doing some math using the formula we talked about in class
on September 21. Specifically,

    target ÷ context = result

Remember that, by default, most browsers set 1em = 16px.

You’ll then use that to compute the values for the CSS styles below.

1. Convert the base font-size listed here from pixels to ems:

      html {
        font-size: 19px;
      }

      19/16 = 1.1875

      html {
        font-size: 1.1875em  /* 18px/16px */
      }

2.  Convert the base font-size listed here to ems, and set the line-height in ems accordingly:

      html {
        font-size: 17px;
        line-height: 24px;
      }

      Font size: 17/16 = 1.0625
      Line height: 24/17 = 1.412

      html {
        font-size: 1.0625em; /* 17px */
        line-height: 1.412em; /* 24px */
      }

3. Set the padding for this page to 12px on top and bottom, and 6px on left and right. Express in
ems:

      html {
        font-size: 1.125em;
        padding:
      }

      So font size is 1.125 * 16 = 18px
      The top and bottom padding is: 12/18 = .666em.
      The left and right padding is: 6/18 = .333em

      html {
        font-size: 1.125em; /* 18px */
        padding-top: .666em; /* 12px */
        padding-right: .333em; /* 6px */
        padding-bottom: .666em; /* 12px */
        padding-left: .333em; /* 6px */
      }

      or

      html {
        font-size: 1.125em; /* 18px */
        padding: .666em , .333em ;/* 6px, 3px */
      }



4. Consider the following CSS. Assuming a browser with its base size at 1em = 16px, how big is h2,
in pixels?

      html {
        font-size: 1.125em;
      }
      figure {
        font-size: 0.888em;
      }
      figure h2 {
        font-size: 1.4375em;
      }

      html font size: 1.125 * 16 = 18px
      figure font size = 18 * .888 = 15.9 (16)
      h2 font-size = 15.9 * 1.4375 = 23px
