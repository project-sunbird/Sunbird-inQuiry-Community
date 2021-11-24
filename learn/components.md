# Components

### Question and Question set service

Question and Question set service is a micro-service which provides APIs to manage the lifecycle and workflows of creation and consumption of question & question set objects.

We use assessment APIs from Sunbird Knowlg for this purpose. (It will be decoupled and moved as part of inQuiry.)

{% hint style="info" %}
[Question and Question set Service API Documentation](http://docs.sunbird.org/latest/apis/questionapi/)
{% endhint %}

{% embed url="https://github.com/project-sunbird/knowledge-platform" %}
Source Code
{% endembed %}

### Question set editor (coming soon)

Question set editor is used to create a question set, configure its behaviour, and add/create questions in the question set. This editor is built in such a way that it is embeddable and extendable.

Today it leverages collection editor from Sunbird Knowlg for this purpose.

{% embed url="https://github.com/Sunbird-Ed/sunbird-collection-editor" %}
Source Code
{% endembed %}

### Question set player

Question set player is responsible for rendering questions & question sets created as per QuML spec. This player is embeddable, configurable and extendable.&#x20;

{% embed url="https://github.com/project-sunbird/sunbird-quml-player" %}
Source Code
{% endembed %}

#### &#x20;<a href="question-set-editor-coming-soon" id="question-set-editor-coming-soon"></a>
