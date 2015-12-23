# githubbot [![NPM version](https://img.shields.io/npm/v/githubbot.svg)](https://www.npmjs.com/package/githubbot)

> Simple github bot with pre-configured methods for handling github webhook payloads.


## Install
Install with [npm](https://www.npmjs.com/)

```sh
$ npm i githubbot --save
```

## Usage

```js
var bot = require('githubbot');
```

## API

### [GithubBot](index.js#L24)
Create a new instance of a GithubBot with provided options.


**Params**

* `options` **{Object}**: Options to configure the github bot.    

**Example**



```js
var bot = new GithubBot();
```



## Events

Array of event types from https://developer.github.com/v3/activity/events/types/

### commit-comment

Github webhook `commit-comment` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#commitcommentevent).

Listen for this event registering a handler with the `.onCommitComment(fn)` method.
Handle events by calling the `.handleCommitComment(payload)` method.

```js
// listen for commit-comment events.
bot.onCommitComment(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the commit-comment event.
bot.handleCommitComment(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### create

Github webhook `create` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#createevent).

Listen for this event registering a handler with the `.onCreate(fn)` method.
Handle events by calling the `.handleCreate(payload)` method.

```js
// listen for create events.
bot.onCreate(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the create event.
bot.handleCreate(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### delete

Github webhook `delete` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#deleteevent).

Listen for this event registering a handler with the `.onDelete(fn)` method.
Handle events by calling the `.handleDelete(payload)` method.

```js
// listen for delete events.
bot.onDelete(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the delete event.
bot.handleDelete(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### deployment

Github webhook `deployment` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#deploymentevent).

Listen for this event registering a handler with the `.onDeployment(fn)` method.
Handle events by calling the `.handleDeployment(payload)` method.

```js
// listen for deployment events.
bot.onDeployment(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the deployment event.
bot.handleDeployment(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### deployment-status

Github webhook `deployment-status` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#deploymentstatusevent).

Listen for this event registering a handler with the `.onDeploymentStatus(fn)` method.
Handle events by calling the `.handleDeploymentStatus(payload)` method.

```js
// listen for deployment-status events.
bot.onDeploymentStatus(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the deployment-status event.
bot.handleDeploymentStatus(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### download

Github webhook `download` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#downloadevent).

Listen for this event registering a handler with the `.onDownload(fn)` method.
Handle events by calling the `.handleDownload(payload)` method.

```js
// listen for download events.
bot.onDownload(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the download event.
bot.handleDownload(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### follow

Github webhook `follow` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#followevent).

Listen for this event registering a handler with the `.onFollow(fn)` method.
Handle events by calling the `.handleFollow(payload)` method.

```js
// listen for follow events.
bot.onFollow(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the follow event.
bot.handleFollow(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### fork

Github webhook `fork` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#forkevent).

Listen for this event registering a handler the `.onFork(fn)` method.
Handle events by calling the `.handleFork(payload)` method.

```js
// listen for fork events.
bot.onFork(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the fork event.
bot.handleFork(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### fork-apply

Github webhook `fork-apply` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#forkapplyevent).

Listen for this event registering a handler with the `.onForkApply(fn)` method.
Handle events by calling the `.handleForkApply(payload)` method.

```js
// listen for fork-apply events.
bot.onForkApply(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the fork-apply event.
bot.handleForkApply(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### gist

Github webhook `gist` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#gistevent).

Listen for this event registering a handler the `.onGist(fn)` method.
Handle events by calling the `.handleGist(payload)` method.

```js
// listen for gist events.
bot.onGist(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the gist event.
bot.handleGist(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### gollum

Github webhook `gollum` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#gollumevent).

Listen for this event registering a handler with the `.onGollum(fn)` method.
Handle events by calling the `.handleGollum(payload)` method.

```js
// listen for gollum events.
bot.onGollum(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the gollum event.
bot.handleGollum(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### issue-comment

Github webhook `issue-comment` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#issuecommentevent).

Listen for this event registering a handler with the `.onIssueComment(fn)` method.
Handle events by calling the `.handleIssueComment(payload)` method.

```js
// listen for issue-comment events.
bot.onIssueComment(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the issue-comment event.
bot.handleIssueComment(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### issues

Github webhook `issues` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#issuesevent).

Listen for this event registering a handler with the `.onIssues(fn)` method.
Handle events by calling the `.handleIssues(payload)` method.

```js
// listen for issues events.
bot.onIssues(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the issues event.
bot.handleIssues(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### member

Github webhook `member` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#memberevent).

Listen for this event registering a handler with the `.onMember(fn)` method.
Handle events by calling the `.handleMember(payload)` method.

```js
// listen for member events.
bot.onMember(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the member event.
bot.handleMember(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### membership

Github webhook `membership` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#membershipevent).

Listen for this event registering a handler with the `.onMembership(fn)` method.
Handle events by calling the `.handleMembership(payload)` method.

```js
// listen for membership events.
bot.onMembership(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the membership event.
bot.handleMembership(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### page-build

Github webhook `page-build` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#pagebuildevent).

Listen for this event registering a handler with the `.onPageBuild(fn)` method.
Handle events by calling the `.handlePageBuild(payload)` method.

```js
// listen for page-build events.
bot.onPageBuild(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the page-build event.
bot.handlePageBuild(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### public

Github webhook `public` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#publicevent).

Listen for this event registering a handler with the `.onPublic(fn)` method.
Handle events by calling the `.handlePublic(payload)` method.

```js
// listen for public events.
bot.onPublic(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the public event.
bot.handlePublic(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### pull-request

Github webhook `pull-request` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#pullrequestevent).

Listen for this event registering a handler with `on-puthe `.on-pull-request(fn)` method.
Handle events by calling the `.handle-pull-request(payload)` method.

```js
// listen for pull-request events.
bot.onPullRequest(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the pull-request event.
bot.handlePullRequest(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### pull-request-review-comment

Github webhook `pull-request-review-comment` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#pullrequestreviewcommentevent).

Listen for this event registering a handler with the `.onPullRequestReviewComment(fn)` method.
Handle events by calling the `.handlePullRequestReviewComment(payload)` method.

```js
// listen for pull-request-review-comment events.
bot.onPullRequestReviewComment(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the pull-request-review-comment event.
bot.handlePullRequestReviewComment(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### push

Github webhook `push` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#pushevent).

Listen for this event registering a handler the `.onPush(fn)` method.
Handle events by calling the `.handlePush(payload)` method.

```js
// listen for push events.
bot.onPush(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the push event.
bot.handlePush(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### release

Github webhook `release` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#releaseevent).

Listen for this event registering a handler with the `.onRelease(fn)` method.
Handle events by calling the `.handleRelease(payload)` method.

```js
// listen for release events.
bot.onRelease(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the release event.
bot.handleRelease(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### repository

Github webhook `repository` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#repositoryevent).

Listen for this event registering a handler with the `.onRepository(fn)` method.
Handle events by calling the `.handleRepository(payload)` method.

```js
// listen for repository events.
bot.onRepository(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the repository event.
bot.handleRepository(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### status

Github webhook `status` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#statusevent).

Listen for this event registering a handler with the `.onStatus(fn)` method.
Handle events by calling the `.handleStatus(payload)` method.

```js
// listen for status events.
bot.onStatus(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the status event.
bot.handleStatus(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### team-add

Github webhook `team-add` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#teamaddevent).

Listen for this event registering a handler with the `.onTeamAdd(fn)` method.
Handle events by calling the `.handleTeamAdd(payload)` method.

```js
// listen for team-add events.
bot.onTeamAdd(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the team-add event.
bot.handleTeamAdd(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```
### watch

Github webhook `watch` event. Find more information about the payload for this event [here](https://developer.github.com/v3/activity/events/types/#watchevent).

Listen for this event registering a handler with the `.onWatch(fn)` method.
Handle events by calling the `.handleWatch(payload)` method.

```js
// listen for watch events.
bot.onWatch(function(payload, cb) {
  // handle payload
  cb(null, payload);
});

// handle a payload for the watch event.
bot.handleWatch(payload, function(err, results) {
  if (err) return console.log(err);
  console.log(results);
});
```

## Related projects
* [base-bot](https://www.npmjs.com/package/base-bot): Simple bot that knows how to handle events when told too. Use base bot to… [more](https://www.npmjs.com/package/base-bot) | [homepage](https://github.com/doowb/base-bot)
* [base-methods](https://www.npmjs.com/package/base-methods): base-methods is the foundation for creating modular, unit testable and highly pluggable node.js applications, starting… [more](https://www.npmjs.com/package/base-methods) | [homepage](https://github.com/jonschlinkert/base-methods)

## Running tests
Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/doowb/githubbot/issues/new).

## Author
**Brian Woodward**

+ [github/doowb](https://github.com/doowb)
+ [twitter/doowb](http://twitter.com/doowb)

## License
Copyright © 2015 [Brian Woodward](https://github.com/doowb)
Released under the MIT license.

***

_This file was generated by [verb](https://github.com/verbose/verb) on December 22, 2015._
