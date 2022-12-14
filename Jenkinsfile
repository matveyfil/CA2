pipeline {
	agent {label "nginx_tst1"}
	stages {
		stage("Checkout") {
			steps{
				git 'https://github.com/matveyfil/CA2'
				echo "Stage 1- Checkout"
				sh "pwd"
			}
		}
		stage("Copy Files to Nginx") {
			steps {
				sh "cp -r * /user/share/nginx/html"
			}
		}
	}
}