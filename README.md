PHPMongoTweet on OpenShift
==========================

This git repository helps you get up and running quickly w/ a PHP sample application
that uses MongoDB on OpenShift

Running on OpenShift
--------------------

Create an account at https://www.openshift.com

Create a php application with mongodb

    rhc app create phpmongotweet php-5.3 mongodb-2

Add this upstream phpmongotweet repo

    cd phpmongotweet
    git remote add upstream -m master git://github.com/openshift-quickstart/phpmongotweet-example.git
    git pull -s recursive -X theirs upstream master


Then push the repo upstream

    git push

That's it, you can now checkout your application at:
    http://phpmongotweet-$yourlogin.rhcloud.com

