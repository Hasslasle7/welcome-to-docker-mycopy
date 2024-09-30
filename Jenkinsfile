node {
    stage('Clone') {
        checkout scm
    }

    stage('Build image') {
        sh "docker build --no-cache -t ${INSTANCE_NAME}:${INSTANCE_TAG} ."
        sh 'curl -H "Authorization: Bearer ${TOKEN}" ${URL}'
    }

    stage('PPost-build') {
        echo "Build and run  Successfully!"
    }
}
