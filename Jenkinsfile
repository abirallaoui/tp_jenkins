pipeline {
    agent any
    
    tools {
        jdk 'JDK 11'  // Assurez-vous d'avoir configuré un JDK dans Jenkins
        git 'Default'  // Assurez-vous d'avoir configuré git dans Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                // Cloner le dépôt GitHub
                git url: 'https://github.com/abirallaoui/tp_jenkins.git', branch: 'main'
            }
        }
        
        stage('Build HelloWorld') {
            steps {
                echo 'Compilation de HelloWorld.java...'
                // Compiler la classe HelloWorld
                sh 'javac HelloWorld.java'
            }
        }
        
        stage('Run HelloWorld') {
            steps {
                echo 'Exécution de HelloWorld.java...'
                // Exécuter la classe HelloWorld
                sh 'java HelloWorld'
            }
        }
        
        stage('Build Merci') {
            steps {
                echo 'Compilation de Merci.java...'
                // Compiler la classe Merci
                sh 'javac Merci.java'
            }
        }
        
        stage('Run Merci') {
            steps {
                echo 'Exécution de Merci.java...'
                // Exécuter la classe Merci
                sh 'java Merci'
            }
        }
        
        stage('Build DeRien') {
            steps {
                echo 'Compilation de DeRien.java...'
                // Compiler la classe DeRien
                sh 'javac DeRien.java'
            }
        }
        
        stage('Run DeRien') {
            steps {
                echo 'Exécution de DeRien.java...'
                // Exécuter la classe DeRien
                sh 'java DeRien'
            }
        }
    }
}
