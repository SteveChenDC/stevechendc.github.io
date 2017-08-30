---
layout: post
title: ActiveRecord ORM and SQL querying
---

## ActiveRecord is an ORM
 Active record is a ORM(Object Relational Mapping) library. This means that even though you're interacting with a database in your Rails app by writing `User.create` or `User.find_by` you're not really writing SQL but writing with a DSL(Domain Specific Language) called ActiveRecord to compile SQL code to interact with the SQL database. So in console I type
{% highlight ruby %}
 User.find_by(id:1)
{% endhighlight %}
 which uses the ActiveRecord Library to execute this hidden SQL code into the database:
 {% highlight SQL %}
 SELECT * FROM users WHERE id = 1 LIMIT 1;
 {% endhighlight %}
This outputs an ActiveRecord hash containing a user found by the query in the database.
{% highlight ruby %}
#<User id: 1, nickname: "Pookie", name: "Renan", user_profile: "http://steamcommunity.com/id/the_real_renan/", user_image: "https://steamcdn-a.akamaihd.net/steamcommunity/pub...", user_location: "Miami, FL, US", uid: "76561198287309916", provider: "steam">
{% endhighlight %}

Here we use the development database from SteamFriend.me to fetch a user with an id of 1.

You can find out more on the official Rails ActiveRecord ORM [here](http://guides.rubyonrails.org/active_record_basics.html)
