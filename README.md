# Artifact-Integration

Integration Steps

1) Login to Jenkins to integrate Artifactory with Jenkins

2) Install "Artifactory" plug-in

3) Manage Jenkins -> Jenkins Plugins -> available -> artifactory

4) Configure Artifactory server credentials

5) Manage Jenkins -> Configure System -> Artifactory

6) Artifactory Servers

7) Server ID : Artifactory-Server

8) URL : Artifactory Server URL

9) Username : admin
   Password : `admin@123
   
   
  ============================================================================================================================================================================
  
  Create a Freestyle Project

1) Create a new job

2) Job Name : artifactory-project

3) Source code management

4) Git URL : get URL here

5) Build Environment

6) Maven3-Artifactory Integration : `<provide Artifactory server and repository details
`

7) Build --> Invoke Artifactory Maven3

- Goals: clean install

Execute job

==============================================================================================================================================================================

Create a Maven Project

1) Create a new job

2) Job Name : artifactory-project

3) Source code management

4) Git URL : get URL here

5) Build Environment

6) Resolve artifacts from Artifactory : <provide Artifactory server and repository details>
  
7) Build - Goals: clean install

8) Post-build Actions

    Deploy Artifacts to Artifactory : <provide Artifactory server and repository details>
    
    Execute job
