pipeline{
  agent any
    properties([parameters([gitParameter(branch: '', branchFilter: '.*', defaultValue: '', description: '', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH')]), pipelineTriggers([pollSCM('')])])
    stages{
      stage("Pull repo"){
        steps{
            git 'https://github.com/ane4ka0205/test.git'
            }
        }
      stage("Hello world"){
        steps{
            sh "mkdir /tmp/folder"
            }
        }
    }
}
