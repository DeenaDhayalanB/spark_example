env.dockerimagename="devopsbasservice/buildonframework:buildon-jenkinsfile"
node {
   stage ('Checkout') {
    checkout scm
    sh 'mvn clean package -DskipTests=True'
  }
   stage ('Build') {
    sh 'mvn clean package -DskipTests=True'
   }

   stage ('SP_Clinic_NexusUpload') {
    sh 'mvn --version'
   }
}
