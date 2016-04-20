---
layout: page
title: Create activity
permalink: /create/
button: true
ref: create
lang: en
published: true
---
You and your friends can edit and create new activities.

To **edit** an activity (did you spot a spelling mistake?) simply follow the *Improve this page* link at the top of most pages on [bettermtl.com](http://bettermtl.com).

To **create** a new activity:

- Create a **New file** in the <code class="highlighter-rouge"><a href="https://github.com/bettermtl/bettermtl.github.io/tree/master/_activities" target="_blank">_activities</a></code> directory
- Copy the example activity bellow to get a head start, you can delete the `[optional]` details which you cannot specify at this time, for example you may not know the `location` yet - come back later to edit and update the activity
- Ensure the file name has the `.md` ending
- **Commit changes** to save

In a few moments, you'll see your changes appear on [bettermtl.com](http://bettermtl.com)

## Example activity
{% highlight markdown %}
---
ref: "reactjs-talk"
title: "ReactJS new year resolutions"
cover: "https://i.imgur.com/rPyXMhl.png"
date: "2017-01-02T17:30:00.000Z"
start_time: "17:30"
end_time: "21:00"
organizer: js-montreal
location: ovh
categories: javascript talk react
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
Specify cofiguration details at the top between `---` and `---`. This structured data tells [jekyll](jekyllrb.com) (the static site generator used to create [bettermtl.com](http://bettermtl.com)) how to process the file.

Name the file in the following format: `YYYY-MM-DD-title.md`

{% highlight markdown %}
# Example of activity file name
2017-01-02-reactjs-talk.md
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

Write your content using markdown right bellow the file config (also known as front-matter data).

## Get more involved:

- [Chat with the community on gitter](https://gitter.im/bettermtl/general)
- Locations (in <code class="highlighter-rouge"><a href="https://github.com/bettermtl/bettermtl.github.io/tree/master/_locations" target="_blank">_locations</a></code>) and people (in <code class="highlighter-rouge"><a href="https://github.com/bettermtl/bettermtl.github.io/tree/master/_network" target="_blank">_network</a></code>) work similarly to activities (in <code class="highlighter-rouge"><a href="https://github.com/bettermtl/bettermtl.github.io/tree/master/_activities" target="_blank">_activities</a></code>)
- [Submit new issues or comments on waffle](https://waffle.io/bettermtl/bettermtl.github.io)
- [Clone the bettermtl.github.io repository](https://github.com/bettermtl/bettermtl.github.io) locally to your machine and hack away at the code.

Great, you are now an active [contributor](https://github.com/bettermtl/bettermtl.github.io/graphs/contributors).

Montrealers all around town appreciate your wonderful help! :-)
