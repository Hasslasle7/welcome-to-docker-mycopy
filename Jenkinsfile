node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t welcome-to-docker-mycopy:dev ."
        sh "curl -H \"Authorization: Bearer mytoken\" localhost:8080/v1/update"
    }

    stage('PPost-build') {
        echo "Build and run  Successfully!"
    }
}
