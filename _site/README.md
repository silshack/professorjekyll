professorjekyll
===============

A collaborative course blog with support for multiple authors.

See the example site deployed on [Github Pages](http://silshack.github.io/professorjekyll).

## Purpose
It's crucial to teach modern programming tools alongside basic coding skills.  Git and Github are valuable and pervasive tools, but they're seldom integrated into programming classes. Enter Professor Jekyll.

Our goal with Professor Jekyll is to make it easy for instructors to set up a collaborative companion blog for their courses.  Students can get comfortable with using [Github Flow in the Browser](https://github.com/blog/1557-github-flow-in-the-browser) (or even a simple push-to-master flow in the very beginning), _in parallel to_ learning their for loops, if statements, and flow of control.  As the course progresses, add in issues, pull requests, and even milestones.

## Usage

For now, these cryptic instructions will suffice:  Clone it, edit the remotes to point to your own GH repo, enable gh-pages, and proceed to edit.

Notably:
* `_config.yml` - this is where you'll define your course and author information
* `_layouts/default.html` - the pages are hard-coded into the header.  You'll also likely want to change the footer a little.
* `css/main.css` - I haven't touched the base CSS beyond some minor tweaks. 

Full documentation should be complete by the end of 2013.

## Contributing
I'd love contributions.  TODOs:
* populate header page links automatically
* little Gravitars for authors everywhere
* Better/distinctive default CSS

Open an issue with your suggestion so we can discuss, or if it's a small one just pull request it.

## Contributors
This project is maintained by Elliott Hauser.

## License
Provided under an MIT License.  See LICENSE.md
