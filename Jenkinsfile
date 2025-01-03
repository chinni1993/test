Pipeline {
agent {
  label 'Tomcat-slave'
}
   Stages{
        stage('Git-checkout') {
        steps {
               git branch: 'main', url: 'https://github.com/chinni1993/test.git'
        }
     }
        stage('Build stage') {
        steps {
               sh 'mvn clean install'
        }
     }
        stage('push to artifactory') {
        steps {
               sleep 15
        }
     }
        stage('deploy') {
        steps {
               sh 'sudo cp /home/ec2-user/jenkins-slave1/workspace/job1/target/*.jar /opt/*tomcat/webapps/'
        }
     }
  }
}
