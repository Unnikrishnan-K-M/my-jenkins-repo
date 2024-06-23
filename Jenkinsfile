//https://github.com/Unnikrishnan-K-M/my-jenkins-repo.git
//https://www.youtube.com/watch?v=AqITZLJ5eZ4

pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Build Application'
            }
        }

        stage('Test') 
        {
            steps 
            {
                echo 'Test Application-2'
            }
        }

        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploy Application'
            }
        }
    }

    post
    {
     
        /* failure
         {
          
            // send failure email

         } */

         always
         {

            // send success or failure email email
            emailext body: 
                                '''Hi Team,
                                Please find the Jenkins pipeline Status here.
                                Thanks!''', 
                                subject: 'Jenkins pipeline Status', 
                                to: 'unnibb208@gmail.com'
         }
    }


}

/* https://www.jenkins.io/doc/book/pipeline/jenkinsfile/ 

 Pipeline syntax - below pipeline script.
    example:
      Email send in case of build failure. (syntax of email)

*/
