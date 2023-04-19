node ('node1'){
    stage ('scm'){
        git 'https://github.com/akashvarma43/spring-petclinic.git'
    }
    stage ('build'){
        sh 'mvn package -DskipTests'
    }
    stage ('post build'){
        archiveArtifacts artifacts: 'target/*.jar'
    }
} 
