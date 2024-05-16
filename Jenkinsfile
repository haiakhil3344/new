pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/haiakhil3344/new.git', branch: 'main')
      }
    }

    stage('install apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('update data') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}