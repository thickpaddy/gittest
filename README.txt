= Gittest

* https://github.com/thickpaddy/gittest

== Description:

Gittest uses your autotest mappings to run tests based on the files
you've created or changed, according to git diff.

== Usage:

Typically, you just execute gittest on the command line. Run it with 
the help option to see what other options are available:

  gittest --help

Of note is the 'commit' option. You can use this to customise the
commit argument to git diff, which defaults to 'HEAD', i.e. the last 
commit. This is really handy when you're working on a topic branch 
and want to run tests based on all the files you've changed in that 
branch, not just those that have been created or modified since the 
last commit. For example:

  gittest -c origin/master
  
You can also create a Gittest instance and both interrogate it and ask 
it to run the tests (this is exactly what the executable does). Have a 
look at the code, it's pretty simple.

== Install:

The latest release should be available from rubygems.org

  sudo gem install gittest

To install directly from source...

  rake install_gem

== License:

(The MIT License)

Copyright (c) 2010 Mark Woods

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
