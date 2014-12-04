# Templates

###HTML files in Meteor define templates

Meteor parses all of the HTML files in your app folder and identifies three top-level tags: `<head>`, `<body>`, and `<template>`.

Everything inside any `<head>` tags is added to the head section of the HTML sent to the client, and everything inside `<body>` tags is added to the body section, just like in a regular HTML file.

Everything inside `<template>` tags is compiled into **Meteor templates**, which can be included inside HTML with `{{> templateName}}` or referenced in your JavaScript with `Template.templateName`.

