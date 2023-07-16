@Library("mylibrary")_
pipeline
{
    agent any
    stages
    {
        stage('ContinuousDownload_master')
        {
            steps
            {
	    	script
		{
			multi.newGit("https://github.com/intelliqittrainings/maven.git")
		}
            }
        }
        stage('ContinuousBuild_master')
        {
            steps
            {
	    	script
		{
			multi.newMaven()
		}
            }
        }
        
     }
 }
       
