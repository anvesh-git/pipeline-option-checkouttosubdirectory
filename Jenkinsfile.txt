pipeline{
    agent any
    options {
		checkoutToSubdirectory('ajsubdir')
	}
    stages{
        stage('Build'){
            steps{
                echo "setting current build to unstable"
            }
        }
    }
}
