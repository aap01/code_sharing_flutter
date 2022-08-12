# Code Sharing Flutter

This is an open source project that aims towards solving challenges, that arise in the process of developing and maintaining multiple projects of similar domain; through discussion and concrete examples. These examples will contain `flutter` and `dart` code.

## What challenges are we talking about?

 - Identify common features among several projects
 - Develop these features in a plug and play fashion while keeping them highly extensible
 - Maintain common dependencies as well as project specific dependencies
 - Establish a connection between the common features and project specific features at minimum effort
 - Easily find and reuse already developed common features at minimum effort
 
## Goals
 - Divide the challenges into smaller pieces
 - Create a morphology for these small challenges
 - Documenting the approaches to solve the small challenges
 - Provide code examples for better understanding of such approaches
 - Thus solving the challenges `without reinventing the wheel`

## Base Project

Let's exploit a "scape goat" to try our ideas on it.
The scape goat project is [Cloud Photo Gallery](https://github.com/aap01/cloud_photo_gallery/tree/scape-goat).

For a clear picture of the context, have a look at the [README.md](https://github.com/aap01/cloud_photo_gallery/tree/scape-goat) of `Cloud Photo Gallery`.
Now, let's add `Cloud Photo Gallery` as a [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) and configure [base_project](/base_project) directory.

Now run this command to populate the contents of [base_project](/base_project) from the `scape-goat` branch of `Cloud Photo Gallery`.

```bash
git submodule update --init
cd base_project
git fetch && git switch scape-goat
cd ..
```

**Note: You might want go through `git submodule` commands.**

