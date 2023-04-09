# .gitattributes

```
Content/** filter=lfs diff=lfs merge=lfs -text
```

## What it do with UE5 project in the git?

The line in your .gitattributes file is specifying that files in the "Content" directory
of your UE5 project should be handled by Git LFS (Large File Storage).

Git LFS is an extension for Git that allows large files to be stored outside the Git repository,
while still being tracked and version-controlled within Git.
This can be useful for projects that have large binary files, such as UE5 projects,
as it can help keep the size of the Git repository manageable.

The "filter=lfs" option in the .gitattributes file specifies that Git LFS should be used to manage
the files in the "Content" directory.
The "diff=lfs" and "merge=lfs" options specify that Git should use the Git LFS command-line
client for diffing and merging changes to these files.

The "-text" option specifies that Git should not attempt to perform any text-based
diffs or merges on the files in the "Content" directory.

Overall, the line in your .gitattributes file is ensuring that large files in the "Content" directory
of your UE5 project are handled by Git LFS, which can help keep your Git repository size manageable
and ensure that large files are properly version-controlled.
