## DevelopingNodes
DevelopingNodes is made with love by Sonu Jose

## Getting Started
Jekyll - ruby based static site generator solution

## Configure Ruby in Windows
- Download Ruby and install in the system
- Install bundler - `gem install bundler`
- Install Related packages - `bundle install`

### Deployment
Firebase hosting
Configurations in the file

**Important:**  For security reasons, Github does not allow plugins (under `_plugins/`) when
deploying with Github Pages. This means:

**1)** Install node packages and generate other necessaries

```bash
$ npm install
$ gulp
```
- Default directory for site generation is `developingnodes-master` 
- The parent directory for deployment purpose only
- The final build will be in the public folder 

**2)** Open Bash in developingnodes-master 
- Running `bundle exec jekyll serve` will generate the files in the public folder
- See configure Ruby on Windows section for handling bundler

**3)** Need to generate site locally (more details below) and push the resulting
HTML (the contents of `_site/` or `../public/`) for firebase deployment. The config.yml has been set to deploy the result into ../public folder for firebase deployment;

**4)** If firebase is not yet configured in the system run `npm install -g firebase-tools`

**5)** Build in the public is deployed to the firebase project
`firebase deploy`

## Thanks

Many thanks to the Ghost team for all the design work. Also many thanks to all contributors,
that help keeping the project alive and updated :smile:

## Copyright & License

Same licence as the one provided by team.

Copyright (C) 2015-2018 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
