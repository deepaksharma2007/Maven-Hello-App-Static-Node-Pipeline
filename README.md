# Two types of parameters in Jenkins 
1. User Defined
2. System Defines

### 1 User-defined variable 
User-defined variables are created by users to store custom values that can be reused within the pipeline. These can be defined in various ways, such as directly in the pipeline script, through Jenkins configuration, or using environment directive.
![image](https://github.com/deepaksharma2007/Maven-Hello-App-Static-Node-Pipeline/assets/64480480/b3c7bd88-1bcc-4908-a194-2965c03c910f)


### 2 System-defined variables 
System-defined variables are built into Jenkins and provide information about the Jenkins environment, the current job, and the build process. Here are some common system-defined variables:

*BUILD_ID:* The current build ID, is identical to BUILD_NUMBER.

*BUILD_NUMBER:* The current build number, an incrementing integer.

*BUILD_TAG:* A unique identifier for the current build, often used for tagging.

JOB_NAME: The name of the currently executing job.

JOB_BASE_NAME: The base name of the job, which excludes the folder path.

BUILD_URL: The URL for the build results.

JOB_URL: The URL for the job.

WORKSPACE: The absolute path of the workspace for the current job.

NODE_NAME: The name of the node the build is running on.

NODE_LABELS: The labels assigned to the node.

EXECUTOR_NUMBER: The unique number of the executor (one per node).

These variables can be accessed in pipeline scripts, shell scripts, or any other type of build script.
