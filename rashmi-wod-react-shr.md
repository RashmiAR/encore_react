---
title: "Rashmi WOD: Encore Saloon in React"
published: true
morea_id: rashmiwod-react
morea_type: experience
morea_summary: "Practice using React."
morea_sort_order: 6
morea_labels: "Rashmi WOD"
---

# Rashmi WOD: Encore Saloon in React

## Background

Encore Saloon is a mezcal bar serving Mexican inspired food at Chinatown, Honolulu.  Your task is to create a rough approximation of the [Encore Saloon website](https://www.encoresaloon.com) using Semantic UI and React.

The mockup created as a result of this practice WOD should look like this:
<img src="rwod-encore-react-solution.png" alt="Encore Saloon website implemented in Semantic UI and React" class="img-responsive">


## Task 0: Download the Semantic UI Mockup

0.1. Download the [Semantic UI Encore Saloon Mockup](rwod-encore-saloon-semantic-mockup.zip) .zip file.  Decompress the file on your computer and open the *index.html* file within.  This should show the mockup of the Encore Saloon home page; you will use React to replicate this mockup.

## Task 1: Set up your development environment

1.1. Create a private GitHub repository named *encore-saloon-react*.  Ensure that there is a README file for the project.

1.2. Clone the repository to your local computer.

1.3. Create a *.gitignore* file in the repository that will ignore `node_modules`, `*.iml`, and `.idea`.

1.4. Create an IntelliJ **Static Web** project within your local *encore-saloon-react* directory.

## Task 2: Create your skeleton Encore Saloon React application

2.1. Navigate to */encore-saloon-react* in the **Command Prompt** (Windows) or **Terminal** (Ubuntu, MacOS).

2.2. Execute `npx create-react-app my-app` to create a new React application.

2.3. Execute `cd my-app`.

2.4. Execute `npm install semantic-ui-react semantic-ui-css --save` to install Semantic UI in this project.

2.5. Execute `del /F src\*` (Windows) or `rm -f src/*` (Ubuntu, MacOS) to remove the unnecessary template files from the *src* directory.

2.6. Copy *styles.css* file for the website, which has classes and properties that may be of use to you.

2.7. Create an *index.js* file in the _/src_ directory with the following contents:

```
import React from 'react';
import ReactDOM from 'react-dom';
import './css/styles.css';
import 'semantic-ui-css/semantic.min.css';
import { Container, Header } from 'semantic-ui-react';

class EncoreSaloon extends React.Component {
  render() {
    return (
        <Container textAlign="center">
          <Header as='h1'>Encore Saloon!</Header>
        </Container>
    );
  }
}

ReactDOM.render(<EncoreSaloon/>, document.getElementById('root'));
```

2.8. You can switch the language version to *React JSX* if IntelliJ prompts you to; you can also disable ESLint.

2.9. Execute `npm start` in your terminal(shell).

2.10. If all is working properly, you should see the **Encore Saloon!** appear at *http://localhost:3000* in your browser.

## Task 3: Build the page

3.1. The *index.html* file is divided into three portions, matching what you did in the previous Semantic UI WOD:

  * The header: the company logo and menubar

  * The middle: full width fluid image.

  * The footer: a footer section with 4 rows.
  
3.2. Create three React components corresponding to these sections in _index.js_ as you did for the Island Snow and Murphy's Bar practice WODs.  Refer to the _index.html_ file provided, or if you prefer you can look back at your own implementation from the UI Frameworks.

3.3. As with the previous WOD, the links on this page do not have to actually work; having the `href` values point to `'#'` or omitted entirely is acceptable for this WOD.

### Hint 1

If you place your images into _/my-app/public_, your relative paths to the images will start in the _public_ folder, ex. `<Image src='/images/wod-7.jpg' />` for an image stored at _/my-app/public/images/wod-7.jpg_.

### Hint 2

Use the `className` attribute to add additional classes to components; some of the examples use this attribute for Semantic UI styles, but you can include your own classes there as well.

## Task 4: Finish

4.1. Ensure that your web page is a reasonable approximation of the expected output.

4.2. Commit and push your finished project to GitHub and verify that your code appears properly on the GitHub site.

4.3. Raise your hands to let me know that you have finished the WOD.

{% include wod-times.html Rx="< 20 min" Av="20 - 30 min" Sd="30 - 40 min" DNF="40+ min" %}

### Submission instructions

You do not have to submit this WOD.

### Footnotes

{% include bit.ly.html url="" %}
