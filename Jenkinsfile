def imagetag = "wmhussain/nginx1.2"

pipeline {
  agent any
  stages {
    node('DockerNode') {
    
    stage('Clone Repository from Github') {
        sh label: '', script: 'rm -rf *'
        sh label: '', script: 'git clone https://github.com/vmvillage/k8sHelloUsingJenkins.git'
    }   
    stage('Build Image') {
        sh label: '', script: 'docker images'
        sh label: '', script: 'echo ${imagetag}'
       // sh label: '', script: 'docker build -t ${imagetag} ./k8sHelloUsingJenkins/'
    }
    stage('Push to DockerHub Account') {
     //   sh label: '', script: 'docker push ${imagetag}'
        
    }
    stage('Delete Image') {
      //  sh label: '', script: 'docker rmi ${imagetag}'
        
    }
}
}
}