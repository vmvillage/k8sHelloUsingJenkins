    node('DockerNode') {
    stages {
    stage('Clone Repository from Github') {
        sh label: '', script: 'rm -rf *'
        sh label: '', script: 'git clone https://github.com/vmvillage/k8sHelloUsingJenkins.git'
    }   
    stage('Build Image') {
        sh label: '', script: 'docker images'
        sh label: '', script: 'echo ${imagetag}'
       // sh label: '', script: 'docker build -t wmhussain/nginx1.2 ./k8sHelloUsingJenkins/'
    }
    stage('Push to DockerHub Account') {
     //   sh label: '', script: 'docker push wmhussain/nginx1.2'
        
    }
    stage('Delete Image') {
      //  sh label: '', script: 'docker rmi wmhussain/nginx1.2'
        
    }
}
}
}