Make folder of that and push into git repo
open jenkins on accessible port
create job
freestyle project -> save
configure-> 
    scm-> git -> repo url 
    branch specifier-> master (or if error occur then main)
    triggers-> poll SCM -> *****
    build steps-> call build.bat
    
