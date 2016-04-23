---
layout: post
title: "Ubuntu Xenial Xerus 16.04 LTS"
excerpt: "Migrate from fedora to Ubuntu"
modified: 2016-03-01
categories: blog  
tags: [linux]
date: 2016-03-01T17:00:00-04:00
comments: true
share: true
author: pooya_golchian
---
**Ubuntu 16.04 LTS release**


You can download this ubuntu from this [link](http://www.ubuntu.com/download/desktop)



**1. After installing**
{% highlight comments %}
sudo apt-get clean all
sudo apt-get update
sudo apt-get upgrade
{% endhighlight %}

**OR**

{% highlight comments %}
sudo apt-get clean all; sudo apt-get update; sudo apt-get upgrade
{% endhighlight %}


**2. Install Flash Player**

{% highlight comments %}
sudo apt-get install flashplugin-installer
{% endhighlight %}
Downlaod .tar.gz package of flash
{% highlight comments %}
sudo wget https://fpdownload.adobe.com/get/flashplayer/pdc/11.2.202.577/install_flash_player_11_linux.x86_64.tar.gz
{% endhighlight %}
{% highlight comments %}
sudo cp libflashplayer.so /usr/lib/mozilla/plugins/
{% endhighlight %}

**2. Install Flash Player**

{% highlight comments %}
sudo apt-get install flashplugin-installer
{% endhighlight %}
Downlaod .tar.gz package of flash
{% highlight comments %}
sudo wget https://fpdownload.adobe.com/get/flashplayer/pdc/11.2.202.577/install_flash_player_11_linux.x86_64.tar.gz
{% endhighlight %}
{% highlight comments %}
sudo cp libflashplayer.so /usr/lib/mozilla/plugins/
{% endhighlight %}
