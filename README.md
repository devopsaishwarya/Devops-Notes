# Devops-Notes
Q/A
......................................................................................................................................
......................................................................................................................................
Git
Q1 - List the SCM's available in the market
A1 - VSS, CVS, Rational clear case, SVN, Perforce, Mercurial, Tortoise SVN, IBM Rational concert, IBM Configuration management, Razor, Quma version control system, Source anywhere, Git etc
.......................................................................................................................................
Q2 - What is Git?
A2 - It is a distributed version control system and a source code management system (SCM) Which as an efficiency to handle small and large size projects effectively. Some of its advantages are 
1) Any project can use GIT without any restrictions.
2)It is calloboration-friendly
3)It has superior disk utilization and network performance.
4)High availability, Data redundancy and replications.
.......................................................................................................................................
Q3 - Difference between GIT and SVN?
A3 - Git is less preferred for handling extremely large files or frequently changing binary files while SVN can handle multiple projects stored in same repository. Git does not support multiple branch commits while SVN Supports multiple branches.
Git is a distributed repository whereas SVN is a centralized repository.SVN is accessible to that Specific Organization whereas Git is accessible to public. 
........................................................................................................................................
Q4 - GIT Advantages
A4 - 1) Any project can use GIT without any restrictions.
     2)It is calloboration-friendly
     3)It has superior disk utilization and network performance.
     4)High availability, Data redundancy and replications.
.........................................................................................................................................
Q5 - List GIT commands
A5 - git config --global user.name "username"
     git config --global user.email "email@example.com"
     git config --list
     git clone
     git --help
     git --version
     git add filename
     git add .
     git commit -m "any message"
     git commit -a -m "anymessage"
     git push
     git pull
     git log
     git status
     git init
     git remote add anyname url_of_empty_repository
     git push origin master
     git branch branchname
     git checkout branchname
     git merge branchname1 branchname2 (master stl)master
     git rebase branchname1 branchname2
     git branch -m old_branch_name new_branch_name // branch rename
     git branch -d branchname1 //delete the merged branch
     git branch -d -r origin/branch_name origin/branch_name origin // to delete the remote branch
     git push origin --delete branchname  // delete the mranch from remote
     git diff
     git revert
     git reset
     git resetgit push origin master --force
     git log --graph --oneline --decorate
     git --help
     git --help command
     git blame filename
     git clean -df
     git -n clean
     git -dn clean
     git ls-files --stage
     git ls-files --cached
     git ls-files --modified
     git ls-files --others
     git ls-files --deleted
     git ls-files --unmergerd
     git ls-files --killed
     git format-patch COMMIT_ID
     git fetch origin
     touch index.css
  ..................................................................................................................................
 Q6 -  List ANT COMMANDS

    ant clean
    ant
    ant compile
------------------------------------------------------------------------------------------------------------------------
 Q7 -  List MAVEN COMMANDS

    mvn archetype:create
   -DgroupId=org.yourcompany.project
   --DartifactId=application
    mvn archetype:create
   -DgroupId=org.yourcompany.project
   --DartifactId=application
    -DarchetypeArtifactId=maven-archetype-webapp

   mvn clean

   mvn validate

   mvn compile

   mvn verify

   mvn install

   mvn clean install

   mvn test

   mvn deploy

   mvn package

   mvn deploy:deploy-file -Dfile=/path/to/jar/file -DrepositoryId=repos-server -Durl=http://repos.company.org/test -DgroupId=javax
  -DartifactId=mail -Dpackaging=jar
  -Dversion=1.0.1


..................................................................................................................................
  GRADLE COMMANDS

  gradle clean
  gradle assemble
  gradle build

....................................................................................................................................

Jenkins
.....................................................................................................................................
.....................................................................................................................................
Q8 - What is jenkins?
A8 - It is a CI/CD tool or a server which is written in java language.
     It provides CI services for software development which can be started via command line or web application. It is free software to        download.
     
Q9 - List the features of jenkins
A9 - Easy installation
     continuous integration and delivery
     Easy configuration
     Extensible
     Distributed ( helps in project deployment)
 ...................................................................................................................................
 Q10 - List of CI Tools 
 A10 - Team city, Travis CI, Bamboo, Gitlab CI, Codeship
       Maven, Ant, Gradle are build technologies
       Jenkins is a continuous integration tool.
  ..................................................................................................................................
  Q11 - The SCM's which jenkins support are
  A11 - Git, CVS, SVN, Mercurial, perforce, clearcase, RTC, AccuRev
  ..................................................................................................................................
  Q12 - Difference between CI tool and Jenkins
  A12 - Jenkins is a free and open source
        It has 1000 + plugins to integrate with a software tool.
        Installation is easy and it uses Java/.net
  ..................................................................................................................................
  Q13 - An example of jenkins pipeline staging
  A13 - 
        pipeline{
                  agent any
        Stages{
               stage('compiling stage') {
               steps {
                    with maven(maven:'maven_3.3.3')
                    sh 'mvn clean compile'
                    }
                }
             }
               stage ('Testing stage') {
              steps {
                      with maven(maven:'maven_3.3.3')
                    sh 'mvn test'
                    }
                 }
             }
                 stage ('Deploying stage') {
              steps {
                      with maven(maven:'maven_3.3.3')
                    sh 'mvn deploy'
                    }
                 }
             }
             
.....................................................................................................................................
.....................................................................................................................................

DOCKER
....................................................................................................................................
.....................................................................................................................................
                    




