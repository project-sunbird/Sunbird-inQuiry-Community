# Question set player

### Getting Started

Question set player library components powered by angular. For help getting started with a new Angular app, check out the Angular CLI.&#x20;

For existing apps, follow these steps to begin using .

### Step 1: Install the packages

```
npm install @project-sunbird/sunbird-quml-player-v9 --save
npm install @project-sunbird/sb-styles --save
npm install @project-sunbird/client-services --save
npm install bootstrap --save
npm install jquery --save
npm install katex --save
npm install lodash-es --save
npm install ngx-bootstrap --save
```

### Step 2: Include the styles, scripts and assets in angular.json

```
"styles": [
...
...
"src/styles.css",
"./node_modules/@project-sunbird/sb-styles/assets/_styles.scss",
"./quml-carousel.css",
"./node_modules/katex/dist/katex.min.css"
],
"scripts": [
...
...
"./node_modules/katex/dist/katex.min.js",
"./node_modules/jquery/dist/jquery.min.js"
]
```

Add following under architect.build.assets

```
 {
    ...
    "build": {
    
    "builder": "@angular-devkit/build-angular:browser",
    
    "options": {
	    ...
	    ...

	    "assets": [
	    
		   ...
		   ...
		    
		    {
			    "glob": "**/*.*",
			    "input": "./node_modules/@project-sunbird/sunbird-quml-player-v9/lib/assets/",
			    "output": "/assets/"
		    }
	    
	    ],

    "styles": [
        ...
        "src/styles.css",
        "./node_modules/@project-sunbird/sb-styles/assets/_styles.scss",
        "./quml-carousel.css",
        "./node_modules/katex/dist/katex.min.css"
    ],
    "scripts": [
        ...
        "./node_modules/katex/dist/katex.min.js",
        "./node_modules/jquery/dist/jquery.min.js"
     ]
    ...
    ...

},
```

### Step 3: Import the modules and components

Import the NgModule where you want to use. Add [question-cursor-implementation.service.ts](https://github.com/project-sunbird/sunbird-quml-player/blob/release-4.5.0/projects/quml-demo-app/src/app/question-cursor-implementation.service.ts)

```
import { CarouselModule } from 'ngx-bootstrap/carousel';
import { QuestionCursorImplementationService } from './question-cursor-implementation.service';
import { QumlLibraryModule, QuestionCursor } from '@project-sunbird/sunbird-quml-player-v9';


@NgModule({
    ...
    
    imports: [ QumlLibraryModule, CarouselModule.forRoot() ],
    providers: [{
        provide: QuestionCursor,
        useClass: QuestionCursorImplementationService
    }]
    
    ...
})


export class TestAppModule { }
```

### Step 4: Add css

Copy both styles.css and quml-carousel.css from below path and add to your application.

```
[styles.css](projects/quml-demo-app/src/styles.css)
[quml-carousel.css](quml-carousel.css)
```

### Step 5: Include the library selector in view( Eg .HTML file)

Use the mock config in your component to send input to Quml player Click to see the mock - [playerConfig](question-set-player.md#undefined) Use 'singleContentRes' for single questionset and 'sectionContent' for section questionset in the mock

```
<quml-main-player [playerConfig]="QumlPlayerConfig" (playerEvent)="getPlayerEvents($event)"
  (telemetryEvent)="getTelemetryEvents($event)"></quml-main-player>
```

### Available components

| Feature     | Notes                      | Selector         | Code                                                                   | Input        | Output                      |
| ----------- | -------------------------- | ---------------- | ---------------------------------------------------------------------- | ------------ | --------------------------- |
| Quml Player | Can be used to render Quml | quml-main-player | _`<quml-main-player [playerConfig]="playerConfig"><quml-main-player>`_ | playerConfig | playerEvent, telemetryEvent |

For More Information, Please refer to the GitHub repo [link](question-set-player.md#getting-started).
