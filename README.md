Etherpad on OpenShift
=====================

This git repository helps you get up and running quickly w/ a Etherpad
installation on OpenShift.  The backend database is MongoDB and the database
name is the same as your application name (using $_ENV['OPENSHIFT_APP_NAME']).
You can name your application whatever you want.  However, the name of the
database will always match the application so you might have to update
.openshift/action_hooks/build.


Running on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/

Then do

    rhc app create etherpad nodejs-0.10 mongodb-2.4 --from-code=https://github.com/wshearn/etherpad-example.git

That's it, you can now checkout your application at (default admin account
is admin/OpenShiftAdmin):

    http://etherpad-$yournamespace.rhcloud.com
