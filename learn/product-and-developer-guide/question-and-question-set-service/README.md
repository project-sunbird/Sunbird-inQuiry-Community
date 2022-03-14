# Question & Question Set Service

Question and Question set service is a micro-service which provides APIs to manage the lifecycle and workflows of creation and consumption of question & question set objects.

In the current implementation, the assessment APIs from Sunbird Knowlg are utilized for this purpose. (It will be decoupled and moved as part of inQuiry.)

#### Key Features:

1. Provides APIs to manage the lifecycle of QuestionSet
2. Generate ECAR file on publishing QuestionSet for offline consumption asynchronously

![Lifecycle Management of a Question Set](<../../../.gitbook/assets/Screen Shot 2022-03-14 at 9.55.13 PM.png>)

{% hint style="info" %}
[Question and Question set Service API Documentation](http://docs.sunbird.org/latest/apis/questionapi/)
{% endhint %}

{% embed url="https://github.com/project-sunbird/knowledge-platform" %}
Source Code
{% endembed %}
