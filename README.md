Hi!

So long story short, I probably should've just forked this: https://github.com/holman/dotfiles/blob/master/bin/cloudapp

...but GitHub doesn't allow you to fork repos if you already have a repo with the same name.  So, instead, here we are.

This is a simple command-line ruby cloudapp client.  Throw it in your $PATH somewhere.

In theory, it should work on OS X, Linux, and Windows.  

In practice, it probably only works in Linux, because that's where I tested it.  Lulz!

It simply uploads a file from the command line to CloudApp and drops the URL into your clipboard.


Installation
-------------

1.  Have ruby.  No ruby? No soup for you.
2.  chmod a+x this thing. 
3.  Add it to your $PATH (or better yet shove the file somewhere that's already in your $PATH)
4.  Requires you set your CloudApp credentials in ~/.cloudapp as a simple file of:
    #   email
    #   password

Usage
-------

1.  cloudapp trololo.png 
2.  Paste that URL! Paste it!


Warranties and such
---------------------

This software (lol, cmon now it's just a script) is provided as-is, so if it causes you any pain or chaos, don't sue me.  

