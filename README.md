
# Gutenberg

This bash script is used for releasing an Nodejs project/module. It follows the best practices of the git-flow.

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
$ bash Release ~/Documents/projects/nirc-lib 1.0.2 Beta
```

Enjoy!
