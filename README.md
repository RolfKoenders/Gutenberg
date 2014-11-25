
# Gutenberg
This bash script is used for releasing an Nodejs project/module. It follows the best practices of the git-flow.

## What?
It takes the project (via the path you specify) and creates the release branch. After that it removes the node_modules/ folder and does a fresh npm install. If that's done it creates the npm-shrinkwrap file and commits it to the release branch. The last stap is merging the release branch to the master branch and create a tag and push it to the server. Optionally it also does an npm publish

## Usage

To use it make sure the package.json file looks correct and you changed the version according to the new version you want to release.

If you use it for the first time, make sure you give it the correct rights

```
chmod +x Release
```

Use it with the following params

```
$1 = Project folder, this folder needs to be a git repo
$2 = Version of the release/tag
Optional: $3 = Release name
Optional: -npm Add this parameter to also fire a 'npm publish' it reads the publish settings from the package.json
```

**example**

```
$ ./Release ~/Documents/projects/nirc-lib 1.0.2 Beta
```

Enjoy releasing!
