@Library('jenkins-shared-library') _

// create variable of map type and set the values

def configMap = [
    component: "payment",
    project: "roboshop"
]
echo "test:"
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pythonEKSPipeline(configMap)
}
else{
    echo "Proceed with CR or NON-PROD pipeline"
}