bdeploy
=======

RELEASE INFORMATION
-------------------
bdeploy 0.9 Beta Release
Released August 26, 2012

OVERVIEW
--------
bdeploy is a simple bash-based deployment script for websites and applications.
With it, you can manage the deployment of files and databases from your test
servers to your live production servers.

USAGE
-----
Just download the main bash script and the example .bdconf file. Place the .bdconf
file in the main, top-level folder of your website or application. Edit the .bdconf
file with the correct configuration and credentials necessary.

From there, you simply need to set up the main folder

./bdeploy -s

add your files to the './current' directory and work on them there. When you are
ready to deploy to the live server, simply run

./bdeploy -d

and it'll do the work for you. It'll keep the different versions of your website
or your application so you can always rollback to the previous version if you need to:

./bdeploy -r

If you want to check the last time you deployed a version, you can run:

./bdeploy -c

And to view the information of your current configuration, you can run:

./bdeploy -i

That's about it. Hope you find the script helpful and useful.
