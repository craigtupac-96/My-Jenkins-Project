pipeline {
    agent any

    stages {
        stage('Fetch') {
		steps {
			echo "Pulling from Github repository"
			git url: 'https://github.com/craigtupac-96/My-Jenkins-Project'
		}
		
        }
        stage('Compile') {
		steps {
			echo "Compiling the java files"
			bat '''
			javac -cp "C:\\Users\\craig\\Hamcrest\\hamcrest-all-1.3.jar";"C:\\Users\\craig\\Junit4\\junit-4.13-beta-1.jar"; "Student.java" "StudentTest.java"
			'''
		}
        }
        stage('Test') {
		steps {
			echo "Running the tests (todo)"
			
		}
        }
    }
}