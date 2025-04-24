// Jenkinsfile
// ----------------------------------------------------------------------
// This is as simple as it gets with declarative pipeline
// ----------------------------------------------------------------------
pipeline {
   agent any
   stages {
      stage('Say Hello') {
         steps {
            echo 'Hello Worlds!'
         }
      }

 		stage('Copy Archive') {
         steps {
             script {
                 step ([$class: 'CopyArtifact',
                 projectName: 'jkpline1',
                 filter: 'target/*.jar',
                 target: 'tmp']);
             	}
         	}
     	}        
   }
}
