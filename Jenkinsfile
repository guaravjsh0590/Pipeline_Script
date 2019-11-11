pipeline {
 agent any
  stages {
  stage('Build') {
   steps {
    echo 'Building the project..'
    git 'https://github.com/guaravjsh0590/Pipeline_Script.git'
    sh '/var/lib/jenkins/workspace/Pipeline_project/build.sh'
   }
  }
  stage('Test') {
   steps {
    echo 'Testing the project..'
    sh '/var/lib/jenkins/workspace/Pipeline_project/test.sh'
   }
  }
  stage('Deploy') {
   steps {
    echo 'Deploying the project....'
    sh '/var/lib/jenkins/workspace/Pipeline_project/deploy.sh'
   }
  }
 }
}
