# TODOs
- create an organisation on github
- create one module for the common scripts
  . setup script
  . update script
  . .. etc ..
- create one module per library
  . curl
  . openssl
  . zlib
  . .. other ..

# structure bins
<pre>
<code>
deps-{crtversion}-{architecture}
            ^
            |
        using PATH
            ^
            |
         app-path
</code>
</pre>

Example:

<pre>
<code>
c:\server-apps\couchdb-1.2-vc9-x64
c:\server-apps\deps-vc9-x64
c:\server-apps\couchdb-1.2-vc9-x86
c:\server-apps\deps-vc9-x86
c:\server-apps\couchdb-1.2-vc6-x86
c:\server-apps\deps-vc6-x86
</code>
</pre>


# structure development tree

See https://wiki.php.net/internals/windows/stepbystepbuild

example:
<pre>
<code>
c:\sdk\couchdb\
        |_ vc9
           |_ x86
           | |_ deps
           | |_ bin
           | |_ lib
           | |_ include
           | |_ couchdb-src
           |_ x64
             |_ deps
             |_ bin
             |_ lib
             |_ include
             |_ couchdb-src
</code>
</pre>
