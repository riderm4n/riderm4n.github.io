---
layout: post
title:  "Install phpmyadmin with nginx as server"
date:   2015-03-18 15:05:00
categories: code
---
<pre>sudo apt-get install phpmyadmin</pre>
<pre>sudo ln -s /usr/share/phpmyadmin/ /usr/share/nginx/www</pre>
<pre>sudo service nginx restart</pre>