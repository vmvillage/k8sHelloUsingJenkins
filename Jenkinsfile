node('DockerNode') {
    stage('build') {
        sh label: '', script: 'rm -rf *'
        sh label: '', script: 'git clone https://github.com/vmvillage/k8sHelloUsingJenkins.git'
    }   
    stage('build') {
        sh label: '', script: 'docker images'
        sh label: '', script: 'docker build -t wmhussain/nginx1.2 ./k8sHelloUsingJenkins/'
    }
    stage('Push to DockerHub') {
        sh label: '', script: 'docker push wmhussain/nginx1.2'
        
    }
    stage('deleteImage') {
        sh label: '', script: 'docker rmi wmhussain/nginx1.2'
        
    }
}