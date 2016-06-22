## Let Me Know Stuff

> A site for displaying syste status information that is stored in a Firebase Database.

### Development Links:

* Local Site: [http://localhost:8000/](http://localhost:8000/):
* Technology References: [Polymer](Polymer.md)

### Polymer Snippets

#### Common Imports

```HTML
<link rel="import" href="../../bower_components/polymer/polymer.html">

<link rel="import" href="../../bower_components/paper-material/paper-material.html">
<link rel="import" href="../../bower_components/paper-card/paper-card.html">
<link rel="import" href="../../bower_components/paper-button/paper-button.html">
<link rel="import" href="../../bower_components/paper-input/paper-input.html">
<link rel="import" href="../../bower_components/iron-autogrow-textarea/iron-autogrow-textarea.html">
<link rel="import" href="../../bower_components/iron-list/iron-list.html">
<link rel="import" href="../../bower_components/iron-icons/iron-icons.html">
<link rel="import" href="../../bower_components/iron-icon/iron-icon.html">
<link rel="import" href="../../bower_components/iron-ajax/iron-ajax.html">
```

#### Firebase Imports

```HTML
<link rel="import" href="../../bower_components/firebase-sdk/index.js">
<link rel="import" href="../../bower_components/polymerfire/firebase-app.html">
<link rel="import" href="../../bower_components/polymerfire/firebase-query.html">
<link rel="import" href="../../bower_components/polymerfire/firebase-document.html">
<link rel="import" href="../../bower_components/polymerfire/firebase-indexeddb-mirror.html">
```

#### Authentication Imports

```HTML
<link rel="import" href="../../bower_components/google-signin/google-signin-aware.html">
<link rel="import" href="../../bower_components/polymerfire/firebase-auth.html">
```

#### Web Component

```HTML
<dom-module id="tm-component">
  <template>
    <style>
      h2 {color:lightgray;}
    </style>
    <paper-material>
      <h2>Component: {{foo}}</h2>
    </paper-material>
  </template>
  <script>
    (function(Polymer) {
      'use strict';
      Polymer({
        is: 'tm-component',
        properties: {
          foo: {
            type: String,
            value: bar,
            notify: true
          }
        },
        ready: function() {}
      });  
    })(window.Polymer);
</dom-module>
```
