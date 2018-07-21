# normalize.css

this is a repo to hold different versions of normalize.css you may need.

This master repo only hold this readme to upgrade add the branches


# normalize.css ready to run files

Downloaded from [https://github.com/necolas/normalize.css](https://github.com/necolas/normalize.css) 
and merged to the "packages" branch to have the versions an application may need.

If you want several versions of normalize.css this will be your primary branch to choose:

    $ git checkout packages

If you just need a special version then checkout the branch you need or create
a new branch including the version you want.

If you need several versions? Then merge it to the packages branch an switch
back to the packages branch.



## Examples/ Howto add new versions


### branch master

    ./README.txt (copy of this readme)


### branch of vA-B-C
    ./vA.B.C/normalize.css
    ./vA.B.C/README.txt (README of normalize.css vA.B.C)
    ./README.txt (copy of this readme)


### Add newer versions

If a new version exists and you need it globaly/ in packages branch:
Don't drop other versions! Add your version to a new branch and merge it to the packages branch


Eg: You need also version 2.0.0:

    $ git checkout master 
    $ git checkout -b "v2-0-0" # (branches needs "-" and NO dots!)
    $ mkdir v2.0.0/
    
    # Download the files *.js/*.css to v2.0.0/
    
    $ git add -a
    $ git commit -m "Adds version 2.0.0"
    $ git push -u origin v2-0-0
    
Now merge the branch to packges branch if you want/need it:

    $ git checkout packages
    $ git merge v2-0-0
    # commit and push, done

Result of packages branch:

    ./vA.B.C/normalize.css
    ./vA.B.C/README.txt
    
    ./v2.0.0/normalize.css
    ./v2.0.0/README.txt
    
    ./README.txt (copy of this readme on creation time)




# Changelog

2018-07

 + Adds version 8.0.0       
 + Init adding normalize.css

