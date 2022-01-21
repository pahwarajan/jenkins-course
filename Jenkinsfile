pipeline {
  agent any
  stages {
    stage('Rajan') {
      steps {
        git(url: 'https://github.com/pahwarajan/mygreenhobbies.github.io.git', branch: '/master', credentialsId: 'github', poll: true)
        readFile '*'
        sh '''#!/bin/bash
cp * /var'''
        echo 'done'
      }
    }

  }
}