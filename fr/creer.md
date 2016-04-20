---
layout: page
title: Publier un sujet ou événement
permalink: /creer/
ref: create
published: true
---
Ajouter un sujet ou événement

Copiez un fichier .md parmi ceux que vous verrez dans le directory `_posts`, changez tous les détails concernés et sauvegardez-le dans le même directory. Laissez vide les champs où vous n'aurez pas de réponse. Par exemple, vous pourrez ne donner ni lieu, ni commanditaire, ni organisateur.

Donc, **pour créer un sujet**, ne donnez ni date ni heure.

Lorsque vous sauvegardez votre nouveau fichier .md dans le directory `_posts` vous devez donner un nom au fichier selon le format suivant :
{% highlight markdown%}
YYYY-MM-DD-title.md
# 2017-01-02-Sujet-Ardent-Debut-Nouvel-An.md  en voici un exemple
{% endhighlight %}
S'il s'agit d'un sujet, nommez votre fichier en donnant une date plusieurs semaines ou mois à l'avenir. Ceci concerne le nom du fichier seulement.


#format de la config du fichier


{% highlight markdown%}
---
#leave this next line as is
layout: post

#Whats the title of your subject or event
title:  "Talk on ES6 JavaScript"

#Url to your cover photo for your event. [optional - default will be used if not given]
cover: "https://frontendmasters.com/assets/es6-logo.png"

#date of the event
date:   2016-02-01 16:04:19 +0000

#start time of the event
start_time: "12:00"

#end time of the event
end_time: "13:00"

#event organizer details
organizer: "Paul Cuciureanu"

#Organiser details go in the _data directory in the community.yml file

#Add your organiser details if you have named an organizer not yet in the data

---
{% endhighlight %}

#Post content

After you have setup your config, all you need to do now is write your content using markdown.

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

- How to get setup with React
- How to get building React Apps
- Bundle your application
- Release your application

If this sounds interesting please register your interest below.


{% endhighlight %}

##Thats all folks
That's all you need to do. Once the website is built again using `jekyll build` or `jekyll serve` your new event will be shown.
