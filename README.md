Etherpad on OpenShift
=====================

Create an account at http://openshift.redhat.com/

Then do

    rhc app create etherpad nodejs-0.10 mongodb-2.4 --from-code=https://github.com/wshearn/etherpad-example.git

That's it, you can now checkout your application at (default admin account
is admin/OpenShiftAdmin):

    http://etherpad-$yournamespace.rhcloud.com
