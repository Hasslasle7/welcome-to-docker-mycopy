node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build -t ${INSTANCE_NAME}:${INSTANCE_TAG} /welcome-to-docker-mycopy/."
        sh 'curl -H "Authorization: Bearer ${TOKEN}" ${URL}'
    }

    stage('PPost-build') {
        echo "Build and run  Successfully!"
    }
}
