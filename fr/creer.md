---
layout: page
title: Publier un sujet sur CapMTL
navigation_title: Publier activité
permalink: /creer/
button: true
ref: create
published: true
---

Adding a topic or event

#Getting started
Créez un fichier .md p.e. en copiant un post existant dans le directory `_posts`. Laisser vide les champs où vous n'aurez pas de réponse. Donc pour créer un sujet, ne donnez ni date ni heure, et possiblement pas de lieu, de commanditaire, d'organisateur.

Le nom que vous donnerez au fichier doit avoir un nom du format suivant, alors choisissez une date des semaines our mois à l'avenir:

{% highlight markdown%}
YYYY-MM-DD-title.md
#Example 2016-01-01-Back-At-Work-After-New-Year.md
{% endhighlight %}

#Config for posts

{% highlight markdown%}
---
#leave this next line as is
layout: post

#Whats the title of your subject or event
title:  "Talk on ES6 JavaScript"

#Url to your cover photo for your event. [optional - default will be used if not given]
cover: "https://frontendmasters.com/assets/es6-logo.png"

#The date of the event
date:   2016-02-01 16:04:19 +0000

#Start time of the event
start_time: "12:00"

#end time of the event
end_time: "13:00"

#event organizer details

#event organizer details
organizer: "Paul Cuciureanu"

#Make sure you setup your Organiser details in the _data directory in the community.yml file

---
{% endhighlight %}

#Post content

After you have setup your config, all you need to do know is write your content using markdown.

#Example Post

{% highlight markdown%}
---
layout: post

#event information
title:  "ReactJS"
cover: "http://blog.addthiscdn.com/wp-content/uploads/2014/11/addthis-react-flux-javascript-scaling.png"
date:   2016-03-28
start_time: "12:00"
end_time: "13:00"

#event organizer details
organizer_email: "david.boyne@test.com"
organizer_name : "David Boyne"
organizer_photo: "https://pbs.twimg.com/profile_images/660943257795457030/igA_joVD.jpg"

---

I will be doing a small talk on an Introduction into ReactJS. We will cover the following:

- What is React?
- How to get setup with React.
- How to get building React Apps.
- Bundle your application
- Release your application

If this sounds interesting please register your interest below.


{% endhighlight %}

##Thats all folks
Thats all you need to do. Once the website is built again using `jekyll build` or `jekyll serve` your new event will be shown.
