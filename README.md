Download Link: https://assignmentchef.com/product/solved-cinf362-week-6-intro-to-responsive-web-design
<br>
<strong>Agenda</strong>

<ul>

 <li>Responsive Web Design (RWD)

  <ul>

   <li>What is it?</li>

   <li>How do we use it?

    <ul>

     <li>Media Queries</li>

     <li>Example</li>

    </ul></li>

   <li>Page Responsiveness Evaluation</li>

  </ul></li>

 <li>Next Week</li>

</ul>




<h2>Responsive Web Design</h2>

<strong>What is it?</strong>

Responsive web design (RWD) is an approach to web design that incorporates a variety of techniques to help pages render on numerous devices depending on screen sizes, orientation, browser, etc. Ideally, the page layout would change based on the previously mentioned factors without forcing any particular view on the user.




<strong>How do we use it?</strong>

Responsive design can be implemented with CSS using multiple methods. The one I will discuss is based on floats which are pretty straight forward. The very first component you need will be located in the &lt;head&gt; tag of your HTML document. It is displayed below:

&lt;meta name=”viewport” content=”width=device-width, initial-scale=1″&gt;

Without this tag, we cannot use <strong>media queries</strong>. Media queries are rules with styles we can place in our CSS that allow us to change elements on our page.

For example, you might have a two-column layout on a desktop that needs to be a single column when displayed on a cellphone. You could use a media query which states that screens smaller than 600 pixels should display the two columns as one. When the screen is larger than 600 pixels, the columns would be displayed separately in two areas.

I’ve provided an example link below the “Additional Reading” with some basic examples of responsive design using floats and inline-block (inline-block can also be used for positioning). Please view the page source or inspect the page for comments in the HTML/CSS with explanations of what’s going on.

<u>Additional Reading</u>

<ul>

 <li><a href="https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag">https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag</a> (Viewport)</li>

 <li><a href="https://developers.google.com/web/fundamentals/design-and-ux/responsive">https://developers.google.com/web/fundamentals/design-and-ux/responsive</a> (General)</li>

 <li><a href="https://css-tricks.com/logic-in-media-queries/">https://css-tricks.com/logic-in-media-queries/</a> (Media Query Logic)</li>

 <li><a href="https://www.smashingmagazine.com/2018/02/media-queries-responsive-design-2018/">https://www.smashingmagazine.com/2018/02/media-queries-responsive-design-2018/</a> (Alternative to floats/media queries)</li>

 <li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox">https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox</a> (Flexbox)</li>

 <li><a href="https://joshnh.com/weblog/why-you-should-use-inline-block-when-positioning-elements/">https://joshnh.com/weblog/why-you-should-use-inline-block-when-positioning-elements/</a> (Argument for inline-block vs floats)</li>

</ul>

<strong><u>Class Example:</u></strong>

<a href="https://iinf362.000webhostapp.com/examples/responsive-design/">https://iinf362.000webhostapp.com/examples/responsive-design/</a>

Make sure to view the source of this page or inspect element. The HTML is explained on the page, but the CSS has comments in it to explain things as well.




<strong><u>If you haven’t done so already, please read the “Creating and Viewing our Web Pages.docx” file on Blackboard. You will not be able to submit anything for the assignment without completing that portion first. </u></strong>

<strong><u> </u></strong>

<strong>Responsive Page Exercises</strong>

Download the “Responsive-Page-Exercises.zip” folder from Blackboard under the Lecture Notes for this week or in the Assignments folder. Inside of this zip folder, there will be two folders.  One will be titled “responsive-fact-page” and the other will be “black-white-responsive-page.” In each of these folders, you’ll find HTML and CSS files. Using the HTML and CSS provided, try to build responsive pages based on the guidelines mentioned below. Below the explanations for each assignment, you’ll find general and assignment-specific guidelines to help you finish the task.

<u> </u>

<u>Responsive Fact Page</u>

Create a web page that will display <strong>6 total facts</strong> about you. The page can start off full width with only one fact being displayed. As the page gets smaller, a new fact should appear until all 6 facts are displayed. Each time a new fact is displayed, the font color of the text should change. Also, the background color of either the body, newly displayed fact, or container (depending on your HTML structure) should be changed as well. <strong>You can also start with a small screen and add facts as it gets bigger. </strong>For this, you would have to reverse your media query logic (use min-width for small to big screen transitions instead of max-width).




The images below depict what part of the page should look like initially, after one media query, and what it should look like at the end. The colors are entirely up to you but try to use white or black for the font, so I can read things more easily. In my version, I decided to use six paragraphs wrapped in a div. Every time a media query was triggered, I would change the paragraph font color and the container color. As long as new facts appear, and some color changes are made, you’ll receive credit for your work.




<u>Responsive Fact Page Tips</u>

<ul>

 <li>Start your media queries from 1200px and then space them out by 150px (1200, 1050, 900, 750, and 600). You can have your “breakpoints” occur whenever you want but these can be a good starting point. If you choose to use these numbers, max-width will be the way to go.</li>

 <li>Have the last 5 facts set to display: none at first and then display them one at a time in each media query (display: block).</li>

 <li>You don’t have to use personal facts if you don’t want to, list any interesting facts if you’d like</li>

</ul>




<u>Black/White Responsive Page</u>

For this part of the assignment, I’ve provided an HTML file with CSS that is already complete. However, this page isn’t very responsive. If you tried to resize the browser, some of the elements will collide or content will become squished. Your task is to add/change CSS in the CSS file to make the page responsive down to 400px. This means that when I resize the browser down to 400px, I should be able to see all content on the page with no horizontal scrollbar being present. There is no “correct” way to approach this which is why no image has been included. Your page should still have all content, but it will be organized differently so it can be viewed on smaller screens.




<u>Black/White Responsive Page Tips</u>

<ul>

 <li>Change “Place Your Name Here” with your name in the two instances on the page</li>

 <li>You can take multi-column layouts and change them to a single column by setting the float property to none and giving the element a width of 100%.</li>

 <li>Max-width: 100% on images will help make them responsive</li>

 <li>Make sure to change pixel widths on some elements to percentages, otherwise containers will overlap or become squished or move when you don’t want them to do so (mentioned again below)</li>

 <li>After changing some widths to percentages, check the margins to make sure margins + width adds up correctly</li>

 <li>There should be no horizontal scrollbar when I look at your page in a smaller browser window</li>

</ul>




<u>General Tips for Responsive Design</u>

<ul>

 <li>Consider your “breakpoints” (where design on your page starts to get a little funky: e.g. text gets crowded, containers start colliding, etc.) and space them appropriately. You don’t need very many to make a page responsive</li>

 <li>Use relative units (give the body a font-size, everything given an em-based value will be based on that initial body value generally)</li>

 <li>Change pixel-based widths to percentages so the containers are more fluid</li>

 <li>If you use media queries going from largest to smallest, use max-width. If you are going from a smaller screen to a larger one, use min-width</li>

 <li>Your smallest media query shouldn’t be below 400px and your largest one shouldn’t be above 1200px at least for this assignment</li>

 <li>Use max-width with containers to ensure they don’t expand past what you’d like. You can use specific pixel-based widths with max-width and percentages with the regular width property (width: 100% and max-width: some pixel amount)</li>

</ul>

To receive credit for this assignment, please submit <strong>two </strong>links to your pages in the assignment submission area. You can find the assignment under the Lecture Notes for this week or in the Assignments folder. One link should direct me to your version of the responsive-fact-page and the other should point to your black-white-responsive-page. Please make sure your CSS is externally placed and that the HTML validates. I will check your work by opening the links you provide and resizing the screen. Check your work before submitting to ensure it is responsive. The links will be due <u>Wednesday, March 4<sup>th</sup>, at midnight.</u>

<strong>Page Responsiveness Evaluation</strong>

Review three websites (1 of my choosing, and 2 that you choose) and discuss the responsiveness of a few pages on those websites. Are the pages responsive on different devices? What components of the websites are done well in terms of mobile design? What areas could be improved? Is a horizontal scrollbar present? Are buttons and other interactive elements sufficiently sized? Do you notice any common components or features across the websites on any platform? How does the page perform when the URL is plugged into the Google mobile-friendly test (<a href="https://search.google.com/test/mobile-friendly">https://search.google.com/test/mobile-friendly</a>)? Base your evaluation on the links provided below which explain responsive web design mistakes in addition to best practices. Feel free to add personal anecdotes about your experiences with mobile versions of websites if you’d like.

<u>Discussion Links</u>

<ul>

 <li><a href="https://uxtricks.design/blogs/ux-design/responsive-design/">https://uxtricks.design/blogs/ux-design/responsive-design/</a></li>

 <li><a href="https://medium.com/level-up-web/best-practices-of-responsive-web-design-6da8578f65c4">https://medium.com/level-up-web/best-practices-of-responsive-web-design-6da8578f65c4</a> (Links to many other tutorials)</li>

 <li><a href="https://www.toptal.com/designers/responsive/responsive-design-best-practices">https://www.toptal.com/designers/responsive/responsive-design-best-practices</a></li>

</ul>

To test each website’s responsiveness, view the websites on different devices (phone, desktop, tablet, laptop, etc.) or use Google Chrome’s web tool to emulate what it would look like on various platforms. To use Google Chrome’s web tool while using a PC, press F12. After this, press Ctrl + Shift + M. This should pull up the responsive tool. You can also right-click the page and select “Inspect Element” to view the web tools. Afterward, you would click the little cellphone/tablet icon (Toggle Device Toolbar) in the top left of the web tool window.

I’ve attached a screenshot below to highlight the button. It is surrounded by a red box and has black text next to it. The other button surrounded by a red box with red text next to it (left side of image) will allow you to change the device you are emulating and viewing the page on.

This link also provides explanations to some of the tools depicted within this screenshot:

<a href="https://developers.google.com/web/tools/chrome-devtools/device-mode">https://developers.google.com/web/tools/chrome-devtools/device-mode</a>