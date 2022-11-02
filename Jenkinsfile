pipeline {
    agent any
   tools{
     maven "maven"
}
   stages{
      stage('git cloning') {
            steps {

      git branch: 'main', url: 'https://github.com/hanumanthu6123/SamplePIP.git'
      }
}
     stage('build'){
       steps {
        sh 'mvn compile'
       }
       }
      stage('testbuild'){
        steps {
            sh 'mvn test'
        }
      }
      stage('packagebuild'){
          steps {
              sh 'mvn package'
          }
          }
      }
        }
