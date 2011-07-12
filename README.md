# Jilles.net
***
Here's the source for my blog. As I base I took Coffecomrade.com's weblog and
went from there. For now, this has not been published at all (jilles.net is
still running the old software). I'm merely using this as a base to experiment
from.

Copyright and -lefts
--------------------
You are allowed to take anything from this site with two exceptions:

* The articles (written human readable content, including images and movies)
* Anything else that ties back to me or this site (think Google Analytics tags,
  Disqus, etc.)

Requirements
------------
Thanks to the braindead native FTP client on Mac OS X, you'll need to install
NcFTP (See: http://www.ncftp.com/ncftp/doc/ncftpput.html) :

    sudo port install NcFTP

In addition ruby-gsl. Installation instructions here:
http://blog.patrickcrosby.com/2010/03/06/ruby-jekyll-lsi-classifier-fixes.html.
Actually, with the newer versions something got fixes somewhere, and the manual
code changes are not necessary anymore.

    sudo port install gsl
    mkdir ~/tmp
    cd ~/tmp
    svn checkout svn://rubyforge.org/var/svn/rb-gsl/trunk
    cd trunk/rb-gsl/
    ruby setup.rb config
    ruby setup.rb setup
    sudo ruby setup.rb install
    sudo gem install classifier
    

Todo's
------
Mainly a list of blogposts I still need to adapt, that I skipped the first pass
(usually images involved).

* Check if iframe is ok at 2006-09-20-quick-post-on-my-ski-plans-this-season.md
* Check if iframe is ok at 2006-09-23-recent-purchases.md
* same for 2008-02-24-skiing.md
* double check presentation embed at 2008-04-28-pfcongrez_marktplaats_architecture.md

Decided to move over my wp-content dir verbatim, so the following ones should
be okay after that:

* Fix image at 2008-10-27-on-user-experience.md
* fix image at 2008-11-15-panolab-iphone-application.md
* Fix image at 2008-11-16-my-social-network-is-changing.md
* 2006-05-19-google-tests-new-feature.md
* 2006-05-28-moola-weekend-millionaires-for-the-rest-of-us.md
* Copy over the map of westendorf and link properly at:
  2006-08-27-map-of-westendorf.md

Also, add GA tag:

<script type="text/javascript">var _gaq = _gaq || [];
 _gaq.push(['_setAccount', 'UA-329999-1']);
 _gaq.push(['_trackPageview']);
 _gaq.push(['_trackPageLoadTime']);

 (function() {
   var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
   ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
   var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
 })();
</script>
