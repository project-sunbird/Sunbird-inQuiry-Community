# Capabilities

In this section, we will cover in a little detail about each of the key capabilities of inQuiry building block.

### **a) Question set editor**&#x20;

is an out of the box tool offered by inQuiry to help you kickstart your creation of **Question Banks**. The key capabilities of this editor are:

* Extendible, pluggable and configurable:&#x20;
  * Plugin based architecture allows you to extend and implement new features with ease.&#x20;
  * Configuration driven \~ Allows you to unleash different capabilities for different workflows.&#x20;
  * Is built using angular tech stack and can be plugged into any portal built using angular. It can also be extended to build native integrations with JS and react frameworks.
* Create new questions or reuse already live questions to stitch a question set with proper metadata tagging.
* Create question sets with multiple sections.&#x20;
* Ability to define the consumption behaviour of the question set. For ex., show hint, solution, set timer etc.
* Ability to preview question set to replicate the actual user experience before publishing it.
* In-built curation workflows to ensure that only reviewed question sets are published.

### **b) Question set services**&#x20;

enable the **End-to-end publishing process**. These are microservices which allow you to: ****&#x20;

* Create, collaborate, curate & publish question(s) and question set(s).&#x20;
* Easily scale as per your needs.
* Unbundled microservices which provide you the flexibility to mix and match to create different solutions using the same set of microservices.

![Representation of services used to power assessments in courses](<../.gitbook/assets/Screen Shot 2022-03-14 at 7.32.10 PM.png>)

### **c) Question editor**&#x20;

enables you to create **diverse question types:**&#x20;

*   inQuiry comes with TWO pre-built question types:&#x20;

    * Multiple choice questions and&#x20;
    * Subjective questions.&#x20;

    It can be extended to build other questions types as per your need.
* Allows you to create questions with rich text, format text, images and math equations amongst others.

### **d) Question set player (QuML player)**&#x20;

is an out of the box player provided by inQuiry to create **engaging & inclusive experiences** for end users consuming the question sets. The key capabilities of this player are:&#x20;

* Extendible, pluggable and configurable:&#x20;
  * Plugin based architecture allows you to extend and implement new features with ease.&#x20;
  * Configuration driven \~ Allows you to configure the player with different capabilities for different workflows.&#x20;
  * Can be plugged into any hybrid mobile app or can be played in web view. Can be extended to build native integrations with JS and react frameworks.
* Inclusive:
  * Built as per the WCAG AA recommendations allowing you to reach a wider audience from day 1.
* Offline & Online:
  * Built to support both online and offline modes of consumption.
* Enables variety of solutions:
  * Allows you to use question sets for different usecases. For ex., the user experience for practice worksheets will show feedback, hints for each question however an assessment will have a completely different consumption behaviour where questions are randomized with a timer.&#x20;
*   Responsive to different resolutions and orientations.&#x20;

    ****

### **e) Analytics:**&#x20;

Every single user interaction is instrumented as per the Sunbird telemetry spec. Therefore, allowing you to use this granular data to create custom reports to turn user actions to insights. Here are the events specific to inQuiry:

* START - start of a question/question set session.&#x20;
* ASSESS - capture score and assessment data.&#x20;
* RESPONSE - capture user responses.&#x20;
* END - end of a question/question set session.

Click [here](https://github.com/sunbird-specs/Telemetry/blob/3.3.0/specification.md) to know more about Sunbird telemetry spec.



### **Additional Information**

Below recording from one of the Sunbird webinars provides more information about the capabilities enabled by inQuiry, the QuML spec, and the technical architecture.

{% embed url="https://www.youtube.com/watch?t=1068s&v=xgvZUfYrxmQ" %}
