
Park Place
=======================

Getting Park Place up and running was a bit of a trick. 
It relies on specific (read: older) versions of a few gems. 
Sounds like a job for [bundler](http://gembundler.com/).

Now to get this running, make sure you have bundler 1.0 installed. 

Clone the repository and:

    $ bundle install
    $ bin/parkplace

And away you go.

*Hat-tip to [jcn](http://pith.org/) and 
[this guy](http://d.hatena.ne.jp/rabbit2go/20100427/1272376003).*

Here are the original docs, if you're into stuff like that:

<pre>
  Park Place                                               an Amazon-S3 clone
  ---------------------------------------------------------------------------

  Okay, so, you've checked out from Subversion and you want to get this suckr
  up and everything.

  First, a checklist:

    1. Do you have Camping and Mongrel installed?

         gem install camping mongrel --include-dependencies

    2. I would also recommend the `sendfile' gem if you're on non-Windows.

         gem install sendfile

    3. Do you have SQLite3 installed?  (If you don't want to mess with the
       database driver.)

         Follow these instructions EXACTLY AS WRITTEN:
         http://code.whytheluckystiff.net/camping/wiki/BeAlertWhenOnSqlite3

  Okay, time to turn it on:

    bin/parkplace

  Once you're sold, you can go ahead and install it for reals:

    sudo ruby setup.rb
    parkplace

  ---------------------------------------------------------------------------
         for more, visit: http://code.whytheluckystiff.net/parkplace
</pre>
