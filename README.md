# 🖼️ 📄 Swift Repository Templates 🖼️ 📄

Helpful file templates and guidance for repositories in github.com/swiftlang. Project maintainers should use this guidance for the root files of every repository. 

## 🌐 SwiftLang GitHub Organization (Org) Level 

There is an organizational level [.github](https://github.com/swiftlang/.github) folder that optimizes for consistency across all repositories. Read more information about GitHub Org Level Files [here](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

- CONDUCT.md**
- SECURITY.md**
- CONTRIBUTING.md (links to [swift.org/contributing](swift.org/contributing))
  
** = special exception from the Core Team in order to opt-out

## 🏠 Repo Level 

The following files are required in each repo and are not set at Org level:
- LICENSE  
  If it's not Apache 2.0, the Core Team will need to approve. GitHub has a [license picker after typing LICENSE in the file name when adding a new file.](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository#applying-a-license-to-a-repository-with-an-existing-license)
- README.md
  
Special Note:
- CONTRIBUTING.md  
  We encourage repo owners to have a custom CONTRIBUTING.md file. Many repos have different review flows, environment set up instructions, testing, and related that may help contributors AND maintainers have a better experience.
- NOTICE or ACKNOWLEDGEMENTS  
  A repository may need to use one of these two files to include license information and more for dependencies, vendored code, etc. Please work with the [Core Team](https://forums.swift.org/new-message?groupname=core-team) to figure out the best course of action here.
  
.github templates:
- codeowners
- pull request template
- issue template

## Contributing
We welcome contributions to this repository! Please read the [Contributor Guide](swift.org/contributing) to get started. If you'd like to propose
a new file, section, or major change, please start with an issue or start a discussion post in the category for the [Contributor Experience Workgroup](https://forums.swift.org/c/contributor-experience/110) on the Forums.
