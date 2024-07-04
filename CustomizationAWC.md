Steps to follow for customizations :

1. Open Teamcenter Command Prompt
     a. Go to %TC_ROOT%/aws2/stage and run initEnv.cmd. (To run tc environment.)
     b. After this, npm run generateModule (To create Module.)
2. Open AWC on browser and change workspace - Active Architect.
3. Run - http://localhost:3000/?dev/showHome and Go to Panel Builder.
4. In Panel builder - create a new panel as desired and move that panel to Panel Builder.
   eg. ItemCreate - move two textboxes for input : id and name and add button. and Save Changes.
5. Open Teamcenter Command Prompt - npm run exportToSrc and select module to modify(This will export source file because of changes made in panel builder into the module.)
6. Open html/json file of module - Go to %TC_ROOT%/aws2/stage/moduleTest/src (src/html and src/viewmodel)
7. Update .json and .html file as per requirement.
8. Go to Teamcenter Command Prompt - awbuild.cmd

9. npm run genSoaApi - for API references. 
