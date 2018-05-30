
## Help

```
npm help command
```

## Search help

````
npm help-search remove
````

## Config options

https://docs.npmjs.com/misc/config

### Default npm init
```
npm set init-author-name "<value>"
```

### List installed
```
npm list
npm list --global true --depth 0
```

### Version numbering

```
<Major Version>.<Minor version>.<Patch>
````

- Major can break functionality
- Minor contains new features but does not break functinality
- Patches are for bugfixes

### Package.json dependencies

^ = Latest of major version
~ = Latest of minor version

### npm install

```
npm install <package-name>
npm install <url>
npm install <path/to/package>
```

### Home page of package

```
npm.im/<packagename>
npm repo <package>
```

### User at npmjs.com

```
npm adduser
```

### Publish to npm

```
git init
git remote add <url>
npm init
npm publish

git tag 1.0.2
git push --tags
```

tag matching tag in package.json. Tags are available at github.com

### Updating a package

1. Make changes to the code
2. Update the version
3. Publish again

Update the version
```
npm version patch
npm version minor
npm version major
```

The npm version command automatically adds a new tag to the git repository and
makes a commit with the version number as message.

Note: The version number of using "npm version" has a "v" as prefix.

Publish the new version:
```
git push
git push --tags
git publish
```

Publishing a Beta

```
version="1.0.0-beta.0"
git add .
git commit -m "message"
git tag "1.0.0-beta.0"
git push
git push --tags
git publish --tag beta
````

### Package info
```
npm info <package>
```


