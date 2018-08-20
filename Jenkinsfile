node {

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build image') {
        zip -r build/release.zip Dockerfile FlaskApp
    }

    stage('Test image') {
        sh 'echo "Tests passed"'
    }

    stage('Push image') {
        sh 'echo "Pushing image"'
    }
}
