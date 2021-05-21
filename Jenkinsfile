node {
stage 'git checkout'
git 'https://github.com/freetechtamil/DevOps-Training.git'

//stage 'Sonar Analysis'
//sh 'mvn sonar:sonar -Dsonar.projectKey=freetechtamil_DevOps-Training -Dsonar.organization=freetechtamil -Dsonar.host.url=https://sonarcloud.io'

stage 'compile'
sh 'mvn compile'

stage 'test'
sh 'mvn test'

stage 'package'
sh 'mvn package'

stage 'archive'
archiveArtifacts 'target/*.war'
}
