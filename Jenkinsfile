node {
    stage('chekout') {
        git 'https://github.com/ajames45/JunitExample.git'
        mvnHome = tool 'M3'
        }

    stage('build') {

        sh "'${mvnHome}/bin/mvn'  clean test"
    }
    
    stage('package')
    {
        sh "'${mvnHome}/bin/mvn' package"
    }
    
} 
