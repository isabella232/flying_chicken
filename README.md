# Flying Chicken

*Coder sounds now in the browser.*

## Built with

 * Coffeescript
 * Node
 * Zappa
     * Express
     * Socket.io
     * CoffeeKup
 
## Register app with Github
1. Visit https://github.com/account/applications/new
2. ?

** Make sure you have the "repo" permission in your oAuth scope

## Install and Run

1. Install Node
2. Install NPM
3. `npm install`
4. `coffee app.coffee`


## Local Testing

To locally simulate a GitHub post-receive hook, enter this in your terminal while running locally :

	curl -d \
	"payload={\"pusher\":{\"name\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"},\"repository\":{\"name\":\"flying_chicken\",\"size\":1148,\"has_wiki\":true,\"created_at\":\"2012-01-20T11:19:23-08:00\",\"private\":false,\"watchers\":4,\"url\":\"https://github.com/codeforamerica/flying_chicken\",\"fork\":false,\"language\":\"JavaScript\",\"pushed_at\":\"2012-06-22T12:41:41-07:00\",\"has_downloads\":true,\"open_issues\":0,\"homepage\":\"\",\"has_issues\":true,\"forks\":1,\"description\":\"Coder sounds delivered to your browsers\",\"organization\":\"codeforamerica\",\"owner\":{\"name\":\"codeforamerica\",\"email\":\"labs@codeforamerica.org\"}},\"forced\":false,\"after\":\"e4a32a2da0050a283e8661159d55f8458e50466f\",\"head_commit\":{\"added\":[],\"modified\":[\"README.md\"],\"author\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"},\"removed\":[],\"timestamp\":\"2012-06-22T12:41:20-07:00\",\"url\":\"https://github.com/codeforamerica/flying_chicken/commit/e4a32a2da0050a283e8661159d55f8458e50466f\",\"id\":\"e4a32a2da0050a283e8661159d55f8458e50466f\",\"distinct\":true,\"message\":\"Added a brief explanation in the read me on how to test post-receive hooks locally using curl.\",\"committer\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"}},\"deleted\":false,\"commits\":[{\"added\":[],\"modified\":[\"config.yml\"],\"author\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"},\"removed\":[],\"timestamp\":\"2012-06-22T11:47:38-07:00\",\"url\":\"https://github.com/codeforamerica/flying_chicken/commit/818e2d1a703422167a7a23d81e81050c6d3bcadf\",\"id\":\"818e2d1a703422167a7a23d81e81050c6d3bcadf\",\"distinct\":true,\"message\":\"Added an Egg to push commits to synstats.herokuapp.com\",\"committer\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"}},{\"added\":[],\"modified\":[\"package.json\"],\"author\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"},\"removed\":[],\"timestamp\":\"2012-06-22T11:57:42-07:00\",\"url\":\"https://github.com/codeforamerica/flying_chicken/commit/7cab977b5de116d5142d9e93540b2931a6f3d324\",\"id\":\"7cab977b5de116d5142d9e93540b2931a6f3d324\",\"distinct\":true,\"message\":\"Updated package.json to include an Engines to hopefully get heroku not \`npm install\` the app properly (cause it's currently crashing out).\",\"committer\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"}},{\"added\":[],\"modified\":[\"README.md\"],\"author\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"},\"removed\":[],\"timestamp\":\"2012-06-22T12:41:20-07:00\",\"url\":\"https://github.com/codeforamerica/flying_chicken/commit/e4a32a2da0050a283e8661159d55f8458e50466f\",\"id\":\"e4a32a2da0050a283e8661159d55f8458e50466f\",\"distinct\":true,\"message\":\"Added a brief explanation in the read me on how to test post-receive hooks locally using curl.\",\"committer\":{\"name\":\"Ben Sheldon\",\"username\":\"bensheldon\",\"email\":\"bensheldon@gmail.com\"}}],\"ref\":\"refs/heads/master\",\"compare\":\"https://github.com/codeforamerica/flying_chicken/compare/54bba782431a...e4a32a2da005\",\"before\":\"54bba782431a8e134b7133c75b94201c326bc7c9\",\"created\":false}" \
	localhost:3000/posthook