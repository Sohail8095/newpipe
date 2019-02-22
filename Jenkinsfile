def workspace
node
{
    stage ("checkout")
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Sohail8095/time-tracker']]])
        workspace=pwd()
    }
    stage ("compile code")
    {
        echo "get the required code for convinent build"
    }
    stage ("buld code")
    {
        echo "Build the extracted code using maven or ant"
    }
    stage ("testing")
    {
        echo "Test the build in an same environment"
    }
    stage ("Deploy")
    {
        echo "Deploy the code in the deploy container"
    }
    stage ("Delivery")
    {
        echo "Deliver it to the main production environment"
    }
}
