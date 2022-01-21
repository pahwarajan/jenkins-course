pipeline {
  agent any
  stages {
    stage('Rajan') {
      steps {
        git(url: 'https://github.com/pahwarajan/mygreenhobbies.github.io.git', branch: 'master', credentialsId: 'github', poll: true, changelog: true)
        sh '''#!/bin/bash
cp blogs.html /var/jenkins_home/workspace/'''
        echo 'done'
      }
    }

  }
}