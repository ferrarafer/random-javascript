Bookmarklet in order to insert jQuery in any page. This is useful if you want to debug a specific page that does not contain jQuery and you think that you could use some of the useful functiones to traverse and manipulate elements.

Based on the results of this question in StackOverflow: [Command for loading jQuery in Google Chrome Inspector?](http://stackoverflow.com/q/9624972/147507)

To install, create a bookmark with this:

    javascript:if(!window.jQuery||confirm('Overwrite\x20current\x20version?\x20v'+jQuery.fn.jquery))(function(d,s){s=d.createElement('script');s.src='https://ajax.googleapis.com/ajax/libs/jquery/1.8/jquery.js';(d.head||d.documentElement).appendChild(s)})(document);
