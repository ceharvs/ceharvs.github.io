---
layout: post
title:  Updating Windows Password with MPI
date:   2014-07-15 16:40:16
description: I recently updated my password on my Windows 7 laptop and then ran into some problems running MPI.  I have MPICH2 Installed and there is a very simple way to update your password in the system if this happens.
---

I recently updated my password on my Windows 7 laptop and then ran into some problems running MPI.  I have MPICH2 Installed and there is a very simple way to update your password in the system if this happens.

{% highlight bash %}

$ mpiexec -register

{% endhighlight %}

Yes, that’s really it!  You’ll be prompted for your username and updated password.  Confirm the password and everything should start working again.