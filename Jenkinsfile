node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t welcome-to-docker-mycopy:${INSTANCE_TAG} ."
        sh 'curl -H "Authorization: Bearer ${TOKEN}" ${URL}'
    }

    stage('PPost-build') {
        echo "Build and run  Successfully!"
    }
}
