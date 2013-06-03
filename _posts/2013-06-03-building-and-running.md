---
layout: entries
title: Building & Running
---
Building and Running
--------------------

### Prequisites
* Compass (SCSS)
* Zurb Foundation 4
* Jekyll

### Getting Started
First, modify the `_config.yml` to meet your site's information. The variables matter most are `site.title`, `site.url`, `site.baseurl`:
{% highlight yaml %}
title : Yojigen
url: /yojigen/
baseurl: /yojigen
{% endhighlight %}
In yogigen's default configuration, the site is hosted under a subdirectory. You may change them to reflect your actual site hierarchy.

When you're done with configuring, put each document under `_posts` folder, where the naming convention is `year-month-day-permalinkUrl`. Choosing `.md` as extension will grant you markdown features, while regardless of document type, Liquid templating syntax are always available. You can find out more in [Jekyll docs](http://jekyllrb.com/docs/templates/).

You should append the following header at the beginning of each file:
{% highlight yaml %}
---
layout: entries
title: <Title>
---
{% endhighlight %}
Note that if you enlist any document under category `Main`, they'll be displayed on the menu bar on top of the page.

Now everything is ready. Run
{% highlight bash %}
jekyll serve -w
{% endhighlight %}
 and launch your browser to `http://localhost:4000/yojigen/`. You should see your docs shown up correctly now.
