#!groovy

node {
    checkout scm
    stage('Build and Deploy') {
        withMaven(maven: 'M3') {
            // skip deploy to nexus to ease tests, don't require a maven settings file with nexus credentials
            // sh "mvn clean install"

            sh "mvn clean install"
        }
    }
}
