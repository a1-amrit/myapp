pipeline{
     agent  any
     stages{
        stage(one){
         steps{
             echo " hi my name is amrit"
             }
             }
      stage (two){
             steps{
             input("do you want toproceed")
             }
             }
      stage(three){
             parallel{
             stage("uit test"){
             steps{
             echo "run time of unit testing"
             }
             }
        stage("intigration test"){
        agent{ 
         docker{
             reuseNode false
             image"ubuntu:latest"
             }
             }
           steps{
            echo  "run time for intigration testing"
            }
            }
          }
          }
          }
          }
          
