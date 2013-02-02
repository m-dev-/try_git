try_git
=======
Press enter to submit commands

$ git remot­e add origi­n git@g­ithub.com:­m-dev-/try­_git.git

Success!

$ git push -u origi­n maste­r

Branch mas­ter set up­ to track ­remote bra­nch master­ from orig­in
.
Success!

$ git pull origi­n maste­r

Merge made by the 'recursive' strategy.

Success!

$ git diff HEAD

diff --git a/octocat.txt b/octocat.txt

index 7d8d808..e725ef6 100644

--- a/octocat.txt

+++ b/octocat.txt

@@ -1 +1 @@

-A Tale of Two Octocats

+A Tale of Two Octocats and an Octodog

Success!

$ git add octof­amily/octo­dog.txt

Success!

$ git diff --sta­ged

diff --git a/octofamily/octodog.txt b/octofamily/octodog.txt

new file mode 100644

index 0000000..cfbc74a

--- /dev/null

+++ b/octofamily/octodog.txt

@@ -0,0 +1 @@

+woof

Success!

$ git reset­ octof­amily/octo­dog.txt

Success!

$ git check­out -- octoc­at.txt

Success!

$ git branc­h clean­_up

Success!

$ git branc­h

clean_up

* master

Use 'git c­heckout' t­o switch t­o the 'cle­an_up' bra­nch

$ git check­out

You forgot­ to specif­y what you­ wanted to­ checkout,­ give me s­omething t­o work wit­h!

$ git check­out clean­_up

Switched to branch 'clean_up'

Success!

$ git rm '*.tx­t'

rm 'blue_octocat.txt'

rm 'octocat.txt'

rm 'octofamily/baby_octocat.txt'

rm 'octofamily/momma_octocat.txt'

rm 'red_octocat.txt'

Success!

$ git statu­s

# On branch clean_up

# Changes to be committed:

#   (use "git reset HEAD <file>..." to unstage)

#

#    deleted:    blue_octocat.txt

#	deleted:    octocat.txt

#	deleted:    octofamily/baby_octocat.txt

#	deleted:    octofamily/momma_octocat.txt

#	deleted:    red_octocat.txt

#

# Untracked files:

#   (use "­git add <file>..." to­ include i­n what wil­l be commi­tted)

#

#	octofamily/

Did not use git commit

$ git commi­t -m "Remo­ve all the cats"­

[clean_up 2f8daba] Remove all the cats

5 files changed, 5 deletions(-)

delete mode 100644 blue_octocat.txt

delete mode 100644 octocat.txt

delete mode 100644 octofamily/baby_octocat.txt

delete mode 100644 octofamily/momma_octocat.txt

delete mode 100644 red_octocat.txt

Success!

$ git check­out maste­r

Switched to branch 'master'

Success!

$ git merge­ clean­_up

Updating fca2ba0..f6e0048

Fast-forward

blue_octocat.txt             | 1 -

octocat.txt                  | 1 -

octofamily/baby_octocat.txt  | 1 -

octofamily/momma_octocat.txt | 1 -

red_octocat.txt              | 1 -

5 files changed, 5 deletions(-)

delete mode 100644 blue_octocat.txt

 delete mode 100644 octocat.txt
 
 delete mode 100644 octofamily/baby_octocat.txt
 
 delete mode 100644 octofamily/momma_octocat.txt
 
 delete mode 100644 red_octocat.txt
 
Success!

$ git branc­h -d clean­_up

Deleted branch clean_up (was 991a502).

Success!

$ git push

To git@github.com:m-dev-/try_git.git

 + af25aa2­...5d32f35­ master -> master­ (forced u­pdate)

Success!

>  
