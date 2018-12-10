pipeline 
{
 agent { label 'linux' }
  stages {
   stage ('Unit Tests') {
    steps {
    sh 'ant -f test.xml -v'
    junit 'reports/result.xml'
    }
   }
   stage ('Build'){
    steps {
    sh 'ant -f build.xml -v'
    }
   }
  }
