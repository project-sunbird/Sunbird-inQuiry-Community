# Server Installation

* The Service can be installed through automation scripts over the server.
* The automation scripts require Ansible as a prerequisite. For server installation components also requires helm as a prerequisite to run the component on Kubernetes.

### :label: **Service Configuration**

* For Service Configuration, Please visit below links:\


{% embed url="https://github.com/project-sunbird/sunbird-devops/blob/master/ansible/roles/stack-sunbird/templates/assessment-service_logback.xml" %}

{% embed url="https://github.com/project-sunbird/sunbird-devops/blob/master/ansible/roles/stack-sunbird/templates/assessment-service_application.conf" %}

### :label: **Service Build Script**

{% embed url="https://github.com/project-sunbird/knowledge-platform/blob/master/build/build.sh" %}

{% embed url="https://github.com/project-sunbird/knowledge-platform/tree/master/build/assessment-service" %}

### :label: **Service Deployment helm Config**

{% embed url="https://github.com/project-sunbird/sunbird-devops/tree/master/kubernetes/helm_charts/core/assessment" %}
