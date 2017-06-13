# Singular Player SDK

This examples show how to use the Singular.live Player SDK.

## INTRODUCTION

The Singular Player SDK provides Java Script libraries to create Singular Player instances, load compositions to the player, 
set payloads for loaded compositions, trigger animations, define and run sequences specified in a json format.

If you want to develop Singular Control Apps, Singular Widgets and Custom data services, please follow the links below:
 - [Singular Widget SDK](https://singularlive.zendesk.com/hc/en-us/articles/115003026388-Singular-Widget-SDK-Documentation)
 - [Singular App SDK](https://singularlive.zendesk.com/hc/en-us/articles/115005838428-Singular-APP-SDK)
 - [Singular REST API](https://singularlive.zendesk.com/hc/en-us/articles/115003104007--REST-API-Description)

## Quick Start

Add the Singular Player SDK path to your html project.

```html
  <!-- Include the Singular Player JavaSrcipt library -->
  <script src="https://libs.singular.live/singularplayer/0.1.1/singularplayer.js"></script>
```

Add iframe pointing to the player url.

```html
  <iframe id="splayer1" src="https://alpha.singular.live/singularplayer/client" 
  style='width:640px;height:320px;border:solid 1px black'></iframe>
 ```

Obtain player object from the iframe by the iframe id.

```html
var player1 = SingularPlayer("splayer1");
 ```

## Example Code

```js
  var player1 = SingularPlayer(“splayer1”);
  var comp = player1.getMainComposition();
  comp.jumpTo(‘In’);
  comp.setPayload({title:’hello world’});
```

## API Reference


## Getting Help

- **Need help**? Ask a question to the [Singular Helpdesk](https://singularlive.zendesk.com/hc/en-us/requests/new).
- **Found a bug?** You can open a [GitHub issue](https://github.com/singularlive/singularplayer-samples/issues).
