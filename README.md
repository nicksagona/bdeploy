bdeploy
=======

RELEASE INFORMATION
-------------------
bdeploy 1.0 Release  
Released August 28, 2012

OVERVIEW
--------
bdeploy is a simple bash-based deployment script for the deployment of
websites and applications. With it, you can manage the deployment of files
and databases from your test server to your live production server.

USAGE
-----
bdeploy is currently for use with the following setups:

### Test Environment     => Live Environment ###
Linux/Unix (w/ bash) => Linux/Unix (w/ bash)  
Windows (w/ cygwin)  => Linux/Unix (w/ bash)

It supports MySQL, PostgreSQL and, of course, SQLite databases. Just download
the main bash script and the example .bdconf file. Place the .bdconf file in
the main, top-level folder of your website or application. Edit the .bdconf
file with the correct configuration and credentials necessary.

From there, you simply need to set up the main folder by running:

./bdeploy -s

Add your files to the './current' directory and work on them there. When you are
ready to deploy to the live server, just run:

./bdeploy -d

and it'll do the work for you. It'll keep the previous versions of your website
or your application as you go along, so you can always rollback to the previous
version by running:

./bdeploy -r

If you want to check the last time you deployed a version, you can run:

./bdeploy -c

And to view the information of your current configuration, you can run:

./bdeploy -i

That's about it. Hope you find the script helpful and useful.
