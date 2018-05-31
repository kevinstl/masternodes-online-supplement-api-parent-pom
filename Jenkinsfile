node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Checkout code from repository
   checkout scm


   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build

   sh "echo NEXUS_PASSWORD: $NEXUS_PASSWORD"

   sh "mvn -s settings-custom.xml clean install deploy"

   //
}
