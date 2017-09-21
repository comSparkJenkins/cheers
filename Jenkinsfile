@Library('spark')
import threeCheers
import repeatMessage
import repeat

pipeline 
{
  agent any
  
  stages 
  {
    stage('Build') 
    {
      steps 
      {
        script 
        {
          for (int i=0; i < 3; i++)
          {
              echo 'Hip, hip hurray!'
          }
        }
 
      }
    }
    
    stage('Analyze')
    {
    	steps
    	{
    		threeCheers()
    	}
    }
    
    stage('Deploy')
    {
    	steps
    	{
    		repeatMessage 3, 'For he\'s a jolly good fellow!'
    	}
    }
    
    stage('Test')
    {
    	steps
    	{
    		repeat(3)
    		{
    			echo 'Celebrate good times!'
    		}
    	}
    }
  }
}
