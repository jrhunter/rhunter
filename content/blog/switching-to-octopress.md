+++
title = "Switching to Octopress"
date = "2012-04-12"
slug = "2012/04/12/switching-to-octopress"
Categories = []
draft = true
+++

[I](http://jroberthunter.com) recently switched from using WordPress to power my personal blog to <a href="http://octopress.org/">Octopress</a>, and my only regret is not switching sooner. Unlike WordPress, MoveableType, or other CMSes, Octopress doesn't require any MySQL processes running in the background, or futzing about with databases. It's a wrapper for <a href="http://jekyllrb.com/">Jekyll</a>, which is a <a href="http://www.ruby-lang.org/en/">Ruby</a> framework for generating blogs as static websites, which are secure, simple and fast.

The advantage of Octopress over Jekyll, from the perspective of a non-developer like me, is that it's simple and straightforward; all you have to do is download and deploy it with a minimum of fuss. In particular, you don't have to write your own CSS, HTML, etc.; all that stuff is automated.

Another advantage (in my case) is that using Octopress is resource- and bandwidth-efficient; since I host this site using <a href="https://www.nearlyfreespeech.net/">NearlyFreeSpeech</a>, I'm only charged when the static site gets visited by a browser, and I don't have to have a MySQL database running constantly in the background.

What's not to like? Well, first and foremost, Octopress is slightly Mac-centric; the author's recommended Ruby version manager is <a href="http://beginrescueend.com/">RVM</a>, which is very Mac-focused and (horrors!) it overwrites shell commands, which seems in my limited experience to be more typical of hacking on OS X than <a href="http://oreilly.com/openbook/freedom/">free</a> platforms like Linux. However, you can also use <a href="https://github.com/sstephenson/rbenv">rbenv</a>, which seems to me to be a much saner way to manage Ruby. Second, theming is still somewhat rudimentary, unless you want to roll up your sleeves and code your own CSS (I don't). But neither of these are huge faults; there are no barriers to using Octopress on a free platform rather than OS X, and hopefully with time an Octopress theming community will begin to flourish.
