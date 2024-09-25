node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t welcome-to-docker-mycopy:dev ."
        sh "curl -H \"Authorization: Bearer mytoken\" 192.168.1.4:8080/v1/update"
    }

    stage('PPost-build') {
        echo "Build and run  Successfully!"
    }
}
