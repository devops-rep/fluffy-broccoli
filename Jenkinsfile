pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Building this from Feature-Branch - App'
            }
        }

        stage('Test') 
        {
            steps 
            {
                echo 'Building this from Feature-Branch - Test App'
            }
        }

        stage('Deploy') 
        {
            steps 
            {
                echo 'Building this from Feature-Branch Deploy App'
            }
        }
    }

    post
    {

    	always
    	{
    		emailext body: 'Summary', subject: 'Pipeline Status', to: 'abc@domain.com'
    	}

    }
}
