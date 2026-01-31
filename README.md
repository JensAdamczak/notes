# notes

Collecting code snippets and information about online articles and books.

## Publish a post

Create content by add a new markdown file with

```
hugo new content/posts/new_file.md
```

Edit the file and test locally with

```
hugo server -D
```

If satisfied set the *draft* flag to false, add tags to the post.

Push changes to master branch. Afterwards publish post via

```
bash publish.sh
cd public
git push --all
cd ..
``` 

Check results at https://jensadamczak.github.io/notes/posts/.

