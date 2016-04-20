---
layout: page
title: Create topic or event activity
permalink: /create/
button: true
ref: create
lang: en
published: true
---
You and your friends can edit and create new activities on [bettermtl.com](http://bettermtl.com).

To *edit* an activity, (maybe you spoted a spelling mistake?), simply follow the "Improve this page" link at the top of most pages.

To *create* a new activity:
- Create a *new file* in the  [`_activities`](https://github.com/bettermtl/bettermtl.github.io/tree/master/_activities) directory 
- Copy the example post bellow to get a head start, and delete the specific details which you cannot specify at this time (maybe location, or time)
- Ensure the file name has the `.md` ending
- You must commit the new file to save the post. In a few moments you'll see it live on [bettermtl.com](http://bettermtl.com)

## Example activity
Copy/paste to your new activity

{% highlight markdown %}
---
ref: "reactjs-talk"
title: "ReactJS new year resolutions"
cover: "http://blog.addthiscdn.com/wp-content/uploads/2014/11/addthis-react-flux-javascript-scaling.png"
date: "2017-01-02T17:30:00.000Z"
start_time: "17:30"
end_time: "21:00"
organizer: js-montreal
location: ovh
categories: lean stratégie entreprise atelier
lang: "en"
---
Happy new year, JS'ers!

Agenda

- What is React?
- Your first ReactJS app
- Bundle and release

[Register here](http://eventbrite.com)
{% endhighlight %}

# The different lines explained
At the top of the file between `---` and `---` specify the front-matter, this structured data tells [jekyll](jekyllrb.com) (the static site generator used to create [bettermtl.com](http://bettermtl.com)) how to handle the new file.

Name the file in the following format: `YYYY-MM-DD-title.md`

{% highlight markdown %}
# Example of activity file name
2017-01-02-hot-topic-tight-after-new-year.md
{% endhighlight %}

# Config for activities
{% highlight markdown%}
---
# reference must be unique, also links different translations together
ref: new-activity-in-la-fontaine-park
# title of the event
title:  "Talk on ES6 JavaScript"
# url for cover photo [optional]
cover: "https://frontendmasters.com/assets/es6-logo.png"
# the date of the activity, should match filename date
date: "2017-01-02T17:30:00.000Z"
# what time does the activity start
start_time: "17:30"
# what time does the activity end
end_time: "21:00"
# organizer ref(erence) defined in the _network directory
organizer: paul-cuciureanu
# location ref(erence) defined in the _locations directory
location: notman
---
{% endhighlight %}

## Activity content

Write your content using markdown right bellow the front-matter config.

## Don't stop here
Locations (in `_locations`) and people/organizational nodes (in `_network`) work in the same way.

Built up your confidence? How to get even more involved:
- [chat with us on gitter](https://gitter.im/bettermtl/general)
- [submit new issues or comments on waffle](https://waffle.io/bettermtl/bettermtl.github.io)
- [clone the bettermtl.github.io repository](https://github.com/bettermtl/bettermtl.github.io) locally to your machine and hack away at the code.

Thank you for being an active contributor!
