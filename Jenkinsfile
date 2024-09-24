node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t welcome-to-docker-mycopy-dev-app ."
    }

    stage('poeost-build') {
        echo "Build and run  Successfully!"
    }
}
