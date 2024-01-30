# Brief discription on Pipelines

<b>PROCESS OF PIPELINE</b>

Pipeline in azure Devops is designed as per project need.
We can increase or decrease number of steps while designing the pipeline

<b>4 steps</b> <br>

Repo <br>
Build<br>
Test<br>
Deploy<br>

<b>Azure pipelines integrates with </b> :
<br>
<br>
GitHub , <br>
GutHub enterprise <br>
Azure repos Git & TFVC <br>
Bitbucket Cloud and <br>
Subversion <br>

<b>Deployment Target </b>: Azure devops can used to deploy your code on multiple targets

<b>Example </b>: <br>
Container registries <br>
VM {Virtual Machine} <br>
Azure Service <br>
Any cloud target <br>
any on - premises <br>

<b>CI & CD in Pipelines : </b> <br>
<b>CI [Continous Integration ] </b>:CI Iis used to automate tests and build for the projects . It is used to find bugs or other build issue in early phase .<br>
<b>CD [ Continous Delivery ] </b>: CD is used to automatically deply and test code in multiple stages ( environments like dev , qa , staging etc .) to maintain the quality . <br>

<b>In simple terms CI is used to build and test the code and CD means to deploy the code </b>

<b>When CI & CD are triggered :</b> <br>
<b>Manually </b>: Anytime you can run the CI , CD pipeline to build and test your code <br>
<b>Automatically </b>: <br>
On each commit <br>
On a fix interval <br>
At a particular time <br>
