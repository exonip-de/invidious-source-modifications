# exonip.de invidious source modifications

The invidious instance exonip.de is not using a modified version of invidious at all and all the source code deployed is directly build from the main branch.

However there is a slight adjustment of some color codes in css file acessed using the 'css/default.css' route. This adjustment has been mode to make the dark mode look better.

As mentioned above no source code of the instance is changed, therefore the file is rewritten using nginx.

This looks something like this:

 <code>   
    location /css/default.css {
        root /var/www/invidious.exonip.de;
    } 
 </code>
