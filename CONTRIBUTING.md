Coding conventions
Start reading our code and you'll get the hang of it. We optimize for readability:

We indent using two spaces (soft tabs)
We use HAML for all views
We avoid logic in views, putting HTML generators into helpers
We ALWAYS put spaces after list items and method parameters ([1, 2, 3], not [1,2,3]), around operators (x += 1, not x+=1), 
and around hash arrows.
This is open source software. Consider the people who will read your code, and make it look nice for them. 
So that we can consistently serve images from the CDN, always use image_path or image_tag when referring to images. 
Never prepend "/images/" when using image_path or image_tag.
Also for the CDN, always use cwd-relative paths rather than root-relative paths in image URLs in any CSS. 
So instead of url('/images/blah.gif'), use url('../images/blah.gif').
