# HTML 5 Features



Web languages need regular upgrades in order to stay current and solve new problems faced by web developers. HTML5 is the latest version of HTML. Below are some HTML5 features you will encounter as you learn with Codecademy.



## `video`



The _video_ element allows you to easily stream video from a website.



```

<video width="450px" height="350px" controls>

 <source src="video-url.mp4" type="video/mp4">

</video>



```



In the HTML above, `width` and `height` set the dimensions for the `video` element. The `controls` attribute creates playback buttons such as "Play" and "Pause". The`source src` tag provides the URL where the video is hosted and `type` specifies the video's type, in this case, "video\/mp4".



## `figure`



_Figure_ elements can be used to display visual content, such as photos, illustrations, diagrams or code snippets.



```

<figure class="gallery-item">

 <img src="image-1.png">

</figure>

<figure class="gallery-item">

 <img src="image-2.png">

</figure>



```



In the example code above, `figure` elements have the class "gallery-item", and each contains an `img` element.



## `section`



_Section_ elements, like divs, can be used to organize webpage content into thematic groups.



```

<section class="contact-form">

 <h2>Contact Us</h2>

 <form>

 ...

 </form>

</section>



```



Above, a `section` element is used to organize `h2` and `form` elements for a website's "Contact Us" feature.



## `nav`



The _nav_ element is used for the part of a website that links to other pages on the site. The links can be organized a number of ways. Below, the links are displayed within paragraph elements. An unordered list could also be used.



```

<nav>

 <p><a href="login.html">Log In</a></p>

 <p><a href="signup.html">Sign Up</a></p>

 <p><a href="contact.html">Contact Us</a></p>

</nav>



```



## `header`



The _header_ element can be used to group together introductory elements on a website, such as a company logo, navigation items, and sometimes, a search form.



```

<header>

 <img src="company-logo.png">

 <nav>

 <p><a href="login.html">Log In</a></p>

 <p><a href="signup.html">Sign Up</a></p>

 <p><a href="contact.html">Contact Us</a></p>

 </nav>

</header>



```



Above, the `header` element encloses the `img` and `nav`.



## `footer`



The _footer_ element is typically found at the bottom or foot of a webpage. It can contain copyright information, links to social media and additional site navigation items.



```

<footer>

 <p>&copy; Acme Granola Corporation 2016<p>

 <div class="social">

 <a href="#"><img src="instagram-icon.png"></a>

 <a href="#"><img src="facebook-icon.png"></a>

 <a href="#"><img src="twitter-icon.png"></a>

 </div>

</footer>



```



Above, between `<footer>` and `</footer>`, copyright information is contained in the `p` element, and social media links are contained within the `div` with class "social".




