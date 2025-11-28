# GCCO Website for Github Pages

Based on the [GCWeb-Jekyll](https://github.com/wet-boew/gcweb-jekyll) repository.


## Usage

Is deployed automatically by the built-in Github Action.

If you wish to create a new page, copy the `_template_$lang.md` file from the root of the repo into somewhere under `_pages/$lang`, update the front-matter accordingly, and add your content.

## Development
To run a development instance, you can use Docker.

Clone this repo, and from the root of the repo, run the following:
```
docker run -it --name GHPages -v "$PWD:/srv/jekyll" -p 4000:4000 -e JEKYLL_UID=`id -u` -e JEKYLL_GID=`id -g` jekyll/jekyll jekyll serve
```

Then browse to [https://localhost:4000](https://localhost:4000), and profit!

If you plan to contribute, you'll need to install the Git pre-commit hook, which ensures the `last_updated` front-matter property is set, and accurately reflects the date/time the page was updated.

To install it, run the following:
```shell
cp git_pre-commit .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

