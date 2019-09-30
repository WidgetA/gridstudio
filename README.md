<img src='http://gridstudio.io/image/logo-grid.svg' width='200px' style='margin-bottom: 30px;'>

Grid studio is a web-based spreadsheet application with full integration of the Python programming language.

It intends to provide an integrated workflow for loading, cleaning, manipulating, and visualizing data. This is achieved through a spreadsheet backend written in Go with integration of the Python runtime to manipulate its contents.

### What is my job?(Widget_A)
This is a tool for our data science team. A user registration function was added.

### Architecture overview
The application is structured in two parts:

1. The (centralized) workspace manager
    1. CRUD interface for creating, copying, editing and deleting workspaces.
    1. Proxy to send traffic to the right workspace environment (part 2)
1. Workspace Go execution environment
    1. Go cell parsing and evaluating spreadsheet backend
    1. Node.js terminal session
    1. Python interpreter integration

For more details about each part check out the code in the repository. If anything is unclear (or unreadable - not all code is equally pretty!) make an issue and details will be provided.

### Installation
To run Grid studio locally refer to the <a href="https://github.com/ricklamers/gridstudio/wiki/Installation">Installation</a> page of the Wiki.

It comes down to pulling the latest Grid studio Docker image that has all dependencies configured (mainly: Go language, Python 3 with packages, Node.js) and starting the Docker container.

For more information check out our <a href="https://github.com/ricklamers/gridstudio/wiki">Wiki</a>.

<b>If don't want to install Grid studio locally you can try out the beta of the hosted version here: <a href="https://dashboard.gridstudio.io">https://dashboard.gridstudio.io</a>.</b>

#### Donate
Like the project? I can dedicate more time to it if you support me:

<a target="_blank" href="https://www.patreon.com/gridstudio"><img src="http://gridstudio.io/image/patron.png" width="176px" /></a>

If you prefer you can also choose to give a one time donation through PayPal:

[![paypal](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XKT365ELJHGMS)

(This is an experiment - if you think I shouldn't run a Patreon/donations for this project let me know in a GitHub issue - I'm very open to feedback!)