So this is my fork of @aashay's fork of @holman's Cloudapp Ruby Script.

Basically, this let's you use cloudapp from the command-line in UNIX systems. You need ruby and gems installed to have this running.

##Installation

### 1) Installing Requirements (for Ubuntu)

    sudo apt-get install ruby1.9.1
    curl http://production.cf.rubygems.org/rubygems/rubygems-1.8.10.zip --O rubygems-1.8.10.zip
    cd rubygems-1.8.10.zip
    sudo ruby setup.rb
    
    sudo gem install cloudapp_api
    sudo gem install mail
    sudo gem install ruby-gmail
    
### 2) Grab the script, copy to /usr/bin and make it executable.

    curl https://raw.github.com/hardikr/cloudapp-rb/master/cloudapp --O cloudapp
    sudo cp cloudapp /usr/bin
    sudo chmod a+x cloudapp

### 3) Create config files ~/.cloudapp and ~/.gmail, both with following format
    username
    password

## Examples

### Upload a file (URL copied to clipboard)
    cloudapp file.txt
    
### Upload a file and email it to john@doe.com
    cloudapp file.txt john@doe.com

## Credits

Huge thanks to:

@dcparker for the ruby-gmail gem. (https://github.com/dcparker/ruby-gmail)

@aaronrussel for the cloudapp\_api gem. (https://github.com/aaronrussell/cloudapp\_api) 

@holman for his original cloudapp dotfile (https://github.com/holman/dotfiles/blob/master/bin/cloudapp)

@aashay for his forked cloudapp script (https://github.com/aashay/CloudApp)


## LICENSE
This is a fork of a couple of scripts, one of them is unlicensed and the other has a license is as follows:

    This software (lol, cmon now it's just a script) is provided as-is, so if it causes you any pain or chaos, don't sue me.  

I don't know if I can add my own license, but if I can, then it is the MIT License

    (The MIT License)
    
    Copyright (c) 2011 Hardik Ruparel
    
    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    'Software'), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
    the following conditions:
    
    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
    IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
    CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
    TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
    SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.