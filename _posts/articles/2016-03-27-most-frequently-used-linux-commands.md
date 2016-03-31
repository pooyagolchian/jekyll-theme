---
layout: post
title: Linux Commands Tips and Tricks
modified:
categories: articles
excerpt: "Linux Lover and SysAdmin Should know"
tags: [linux]
comments: true
share: true
author: pooya_golchian
image:
  feature:
date: 2016-03-27T20:04:47+04:30
---
This post update every day! You can follow this article and learn linux command tips and tricks. Enjoy :)./var

**1. tar command examples**

Create new tar archive
{% highlight Commands %}
$ tar cvf archive_name.tar dirname/
{% endhighlight %}

Extract from an existing tar archive.
{% highlight Commands %}
$ tar xvf archive_name.tar/
{% endhighlight %}

View an existing tar archive.
{% highlight Commands%}
$ tar tvf archive_name.tar
{% endhighlight %}

**2.grep command examples**

Search for a given string in a file (case in-sensitive search).
{% highlight Commands%}
$ grep -i "the" demo_files
{% endhighlight %}

Print the matched line, along with the 3 lines after it.
{% highlight Commands%}
$ grep -A 3 -i "example" demo_text
{% endhighlight %}

Search for a given string in all files recursively
{% highlight Commands%}
$ grep -r "pooya" *
{% endhighlight %}

**3.find command examples**

Find files using file-name ( case in-sensitve find)
{% highlight Commands%}
# find -iname "MyCProgram.c"
{% endhighlight %}

Find all empty files in home directory
{% highlight Commands%}
# find ~ -empty
{% endhighlight %}

**4. ssh command examples**

Login to remote host
{% highlight Commands%}
ssh -l jsmith remotehost.example.com
{% endhighlight %}

Debug ssh client
{% highlight Commands%}
ssh -v -l jsmith remotehost.example.com
{% endhighlight %}


Display ssh client version
{% highlight Commands%}
$ ssh -V
OpenSSH_7.2p2 Ubuntu-1, OpenSSL 1.0.2g  1 Mar 2016
{% endhighlight %}

**5. Vim (Vim is an advanced text editor)**

Go to the 143rd line of file
{% highlight Commands%}
$ vim +143 filename.txt
{% endhighlight%}

Go to the first match of the specified
{% highlight Commands%}
$ vim +/search-term filename.txt
{% endhighlight%}

Open the file in read only mode.
{% highlight Commands%}
$vim -R /etc/passwd
{% endhighlight%}

**6. diff command**

Ignore white space while comparing.
{% highlight Commands%}
# diff -w name_list.txt name_list_new.txt

2c2,3
< John Doe --- > John M Doe
> Jason Bourne
{% endhighlight%}

**7. ls command (list directory contents)**

Display filesize in human readable format (e.g. KB, MB etc.,)
{% highlight Commands%}
pooya@pooya-ThinkPad-Edge-E430:~$ ls -lh
total 1.8G
drwxrwxrwx 13 pooya pooya 4.0K Sep 21  2015 android-sdks
drwxrwxr-x  7 pooya pooya 4.0K Aug 19  2015 android-studio
drwxrwxrwx  3 pooya pooya 4.0K Mar 19 11:14 design
drwxr-xr-x  2 pooya pooya 4.0K Mar 21 01:52 Desktop
drwxr-xr-x  2 pooya pooya 4.0K Mar 19 11:02 Documents
drwxr-xr-x  3 pooya pooya 4.0K Mar 23 21:36 Downloads
-rwxrwxrwx  1 pooya pooya 8.8K Feb 25 23:28 examples.desktop
{% endhighlight%}
