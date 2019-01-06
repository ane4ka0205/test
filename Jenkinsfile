pipeline{
  agent any    
    stages{
      stage("Pull repo"){
        steps{
            git 'https://github.com/ane4ka0205/test.git'
            }
        }
      stage("Hello world"){
        steps{
            sh '''
            set +xe
            mkdir /tmp/folder
            touch /tmp/file1
            '''
            }
        }
    }
}
