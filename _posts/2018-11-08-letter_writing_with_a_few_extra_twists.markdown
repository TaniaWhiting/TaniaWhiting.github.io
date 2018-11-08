---
layout: post
title:      "Letter Writing with a Few Extra Twists"
date:       2018-11-08 16:48:21 -0500
permalink:  letter_writing_with_a_few_extra_twists
---


Dear Mom,

Let me give you some insight about HTML and how to create your own webpages.  You know how you love to write letters to friends and family?  Okay, it's pretty much the same but with a few additional twists to the writing .  First off,  pull out an old letter of yours and we will make that document World Wide Web ready in no time at all.  Once you get the hang of it, it won’t just be friends and family that can read your letters, but anyone online in the world!

The language of the web is HTML, or more explicitly, Hypertext Markup Language.  All text must be marked up in this language for the browser to display the content you have created in your webpage.  So to begin with, we will literally mark up your letter in HTML and this is done using tags.  A tag takes the following form, <tag>.  The tags usually come in pairs with an opening and a closing tag surrounding the text we want to mark up.  As our first example of using tags, let’s  give your letter the heading  “Our Summer Vacation!”.  To do so we will surround the text with the h1 header tag, a tag which will provide the largest text size, making sure the heading will stand out.  Visually it looks like this:

<h1>Holidays with the Family!</h1>
 
 Congrats on your first line of HTML, Mom!  Okay, let’s forge on ahead!  One of the most common structural  elements in any written document is the paragraph.  HTML marks paragraphs with the paragraph tag, <p>.  So let’s now add the following tag to the front of the each paragraph in your letter.  At the very end of each paragraph, place the closing tag </p>.  Okay, so at this point, we have marked up your letter for a heading and paragraphs.  Not too tough, right?!  
 
Does your letter have more than one page?  No problem!  We can link to each additional page using the anchor tag, <a>, which defines a hyperlink.  This is a little more complex because we have to also include an attribute known as the href attribute to provide the destination we are linking to, in this case the extra page in your letter.  It might look something like this:  <a href=”https://www.MomsLetters.com”>Mom’s Letter Page 2!</a>.  We can link to as many pages as you have in your letter and they will all successfully link to one other.

Now, Mom, don’t you often include in your letters photographs?  Well, we can add those too!   Including them is easy, we just use the HTML image tag, <img>.  This again is a litte more complex because it also has  an attribute, the src attribute  which provides  the location of the image we want to display.  As an example, we could write the following for one of your photos:  <img src=”HolidayPhoto.jpg” alt=”Holiday Photo 1”>.  Notice that in HTML the img does not have a closing tag.  The alt attribute that we have included just provides some user friendly text in case the image does not successfully render.

Okay Mom, we are really zooming along here now.  We just need some additional information to make the page fully functional.  Everything we have so far discussed goes in the body of the HTML page, which again will go between tags, in this case the body tags.  We also have to include <!DOCTYPE html> at the very top of the page, and HTML head tags that contain metadata about the HTLM document itself.  Visually it will look like this:

<DOCTYPE! html>
<html>
	<head>
               </head>	
               <body>
                                        Your letter goes in here Mom!
               </body>
</html>

Well Mom I hope you can see getting published online is really as easy as writing a regular letter, just with a few additional twists.  Doesn’t matter what you want to say or show with pictures, it’really is quite easy to generate on online presence.  See you online Mom!

