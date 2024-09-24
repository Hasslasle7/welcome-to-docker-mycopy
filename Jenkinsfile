node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t welcome-to-docker-mycopy-dev-app ."
    }

    stage('poost-build') {
        echo "Build and run  Successfully!"
    }
}
