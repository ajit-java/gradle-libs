This https://github.com/ajit-java/gradle-libs project is an example of grale project created via gradle init, where library project is part of same git repo.

This https://github.com/ajit-java/gradle-libs-subrepo is an example of project where git subrepo add on is used to maintain git libs, it creates a gradle-libs-subrepo/utilities/.gitrepo file which contains gitsubrepo configs. 

## gradle init
https://docs.gradle.org/current/samples/sample_building_java_applications_multi_project.html

## git submodules 
https://stackoverflow.com/questions/18748436/is-it-possible-to-declare-git-repository-as-dependency-in-android-gradle

## git sub-repo project & 2 separate git repos examples
https://stackoverflow.com/questions/4659549/maintain-git-repo-inside-another-git-repo
this is by far the best as it allows to maintain two repos and breakpoints can be added for debugging.
Note: git subrepo would just download the remote project, it must be registered to gradle as library in build.gradle file. 
 


## gradle source dependencies
https://blog.gradle.org/introducing-source-dependencies
this option is ok in the sence gradle would download and build both projects, but there is no way to add a breakpoint in sub projects.