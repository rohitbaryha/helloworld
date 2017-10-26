!groovy

node {

stage 'Checkout'
	checkout scm

stage 'Setup'
	sh 'npm install'

stage 'Test Mocha'
	sh './node_modules/mocha/bin/mocha'

stage 'Cleanup'
        echo 'prune and cleanup'
        sh 'npm prune'
        sh 'rm node_modules -rf'
}
