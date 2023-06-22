pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the first build job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'this is the second test job'
        sh 'npm test'
      }
    }

<<<<<<< HEAD
// uncomment the following lines by removing /* and */ to enable
     tools{
       nodejs 'nodejs' 
=======
    stage('package') {
      steps {
        echo 'this is the third package job'
        sh 'npm run package'
      }
>>>>>>> 765124227526ee030fc2495f974df7805f597fc0
    }

    stage('') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed by code.'
    }

  }
}