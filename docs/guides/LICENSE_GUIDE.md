# License Guide

Make applicable license conditions transparent.

> [!TIP]
> More information is available from [GitHub documentation][github-documentation].

## Choosing a license

The following [online guide](https://choosealicense.com/) is an excellent way to pick a license.

## Adding a license

Add a file called `LICENSE` to the root of your repository, the `docs` folder, or the `.github`
folder, with the text of the license you chose. GitHub automatically adds a link to this file in the
_About_ section of your repository homepage.

You can either repeat the license in each file requiring it but this is generally cumbersome. To
make your life easier you can use the following reduced license instead, which points to the main
license file for more information:

```
//
//  Copyright (c) SRG SSR. All rights reserved.
//
//  License information is available from the LICENSE file.
//
```

Avoid dates in license information since they have no real values and are likely never correctly
updated.

[github-documentatiojn]: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository
