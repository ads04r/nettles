nettles
=======

A friend of mine had her Facebook account hacked. I retaliated.

The idea is simple - if you come across a fake login page for an online
service, run ./bin/sting [url] , where [url] is the URL of the fake
page. The script will invent a bogus username and password and try to
log in.

What's the point?
-----------------

Most of these pages log the username and password of those unlucky
enough to be duped by them. Every time you run this script, that
particular page registers login credentials that are bogus and can't
be used. Run it a few times, preferably from different IP addresses,
and suddenly the stolen credentials are starting to fill with rubbish
that the scammer can't use. So by running this script several times
(perhaps at random intervals from cron!) you're reducing the efficiency
of that particular fake login page.

