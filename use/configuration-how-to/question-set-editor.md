# Question set editor

### Getting Started

Question set editor library components powered by angular. For help getting started with a new Angular app, check out the Angular CLI.&#x20;

For existing apps, follow these steps to begin using .

### Step 1: Install the packages

```
npm install @project-sunbird/sunbird-collection-editor-v9
```

### Step **2**: Install the packages

**Step 1: Install the following packages**

```
npm install @project-sunbird/sunbird-collection-editor-v9
```

### Step 2: Include the assets in angular.json

```
"assets": [
          "src/favicon.ico",
          "src/assets",
          {
            "glob": "**/*",
            "input": "./node_modules/@project-sunbird/sunbird-collection-editor-v9/lib/assets/",
            "output": "/assets/"
          }
        ],
```

### Step **3**: Import the modules and components

Add to `NgModule` for the application in which you want to use:

```
import { CollectionEditorLibraryModule } from 'sunbird-collection-editor-v9';


@NgModule({
    ...
    imports: [
        CollectionEditorLibraryModule,
    ...
})
```

### Step 4: Include the library selector in view( Eg .HTML file)

```
<lib-editor [editorConfig]="editorConfig" (editorEmitter)="editorEventListener($event)" ></lib-editor>
```

Sample editorConfig:

```
editorConfig: {
    context: {
        identifier: 'do_1132125506761932801130',
        user: {},
        framework: '',
        channel: '',
        uid: "
    },
    config: {
        mode: 'edit', // edit / review / read
        maxDepth: 0,
        objectType: 'QuestionSet',
        primaryCategory: 'Practice Question Set',
        isRoot: true,
        iconClass: 'fa fa-book',
        children: {
            Question: [
                'Multiple Choice Question',
                'Subjective Question'
            ]
        },
        hierarchy: {}
    }
}
```

For More Information, Please refer to the GitHub repo [link](https://github.com/Sunbird-Ed/sunbird-collection-editor/tree/release-4.5.0)
