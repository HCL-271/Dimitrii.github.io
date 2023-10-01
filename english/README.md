# Fork this repo for create your own web CV. ([На русском](https://HCL-271.github.io/))  ([English](https://HCL-271.github.io/english/)) 
Launch your resume site without server on github pages! Optional need a domain name.

# Configuration

* Fork this repo as `<you_github_nickname>.github.io`
* Setup your domain (may skip this step and site be on `<you_github_nickname>.github.io`)
  * Create CNAME subdomain record on your DNS provider:
    * `cv` -> `<you_nickname>.github.io`
  * Open fork repository settings
  * Go to `Pages/Custom domain` enter you `cv.<example.com>` (And enforce HTTPS)
  * Change [CNAME-file](https://github.com/HCL-271/HCL-271.github.io/blob/main/CNAME) in fork with your subdomain: `cv.<example.com>`
* Change left side with your information via [_config.yml](./_config_eng.yml) like this:
  ```yaml
  fullname: Dmitrii Kovrizhnukh
  favicon: /assets/images/favicon.svg
  logo: /assets/images/ebA-_ztGqQk.jpg
  
  show_info: true # Show block with information
  age: 22 y.o.
  location: Moscow, Russia
  language: Russian, English, ein bißchen Deutsch
  
  show_contacts: true # Show block with buttons
  mailto: mailto:kovrizhnykh.diu@phystech.edu
  cv_pdf_link: [Resume_CV](https://github.com/HCL-271/HCL-271.github.io/edit/main/pdf/hcl-271_github_io_.pdf)
  
  # Don't change this
  remote_theme: annndruha/minimal-resume
  plugins:
  - jekyll-remote-theme
  ```
* Change [index.md](./english/index.md) with you information
* Change `/assets/images/photo.png` and pdf link
* Wait a minute for GitHub-actions auto build and enjoy your site 😋!


# Extra

This site required page theme [minimal-resume](https://github.com/Annndruha/minimal-resume) which is in the [_config.yml](./english/_config_eng.yml) as remote_theme.

Site hasn't got a pdf converter, manually update the pdf file: [cv_pdf.pdf](https://github.com/HCL-271/HCL-271.github.io/blob/main/pdf/Dmitrii%20Kovrizhnukh.pdf)
