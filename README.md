##Frontend-common Components: Exploring Possible Management Solutions
*Documentation for the Private-bower app can be found [here](http://hacklone.github.io/private-bower) & original repo [here](https://github.com/Hacklone/private-bower)*

###Private Bower Server Solutions:
- example currently live at http://enigmatic-ocean-8756.herokuapp.com
- build processes need to specify that a remote bower server will be used (done via .bowerrc file) 

#####Private bower server w/ hosted zip
Should work, but produces: `bower ENORESTARGET URL sources can't resolve targets` on `bower install`
- Files are still technically public, but are not indexed anywhere and can only be pulled when their URL is directly referenced or the private bower registry is used. 
- Zip must be pushed to the hosted location every time an update is made.

#####Private bower server w/ private GitHub repo
Not going to work. Requires inputing of GitHub credentials during build process. 

#####Private bower server w/ public GitHub repo
Works, but repo must be publicly available. 

###Local Solution:
#####Directly referencing private GitHub repo in bower file
Not going to work. Requires inputting of GitHub credentials during build process