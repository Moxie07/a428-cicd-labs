node {
    env.NODEJS_HOME = "${tool 'NodeJS 16'}"
    env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    stage('Build') {
        sh 'npm install'
    }
    stage('Test') {
        sh './jenkins/scripts/test.sh'
    }
}