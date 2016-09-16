# Jekyll source for my home page

(c) 2016 Arrvindh Shriraman

* Layout based on one-page-wonder(https://startbootstrap.com/template-overviews/one-page-wonder/) 
* Further modifications by me are [licensed](LICENSE.md).
* Feel free to reuse anything except site content:
  * `assets/images`,
  * `_posts/*`,
  * `*.md`.
* To copy to SFU:
    jekyll build --config=_config.yml,_sfuconfig.yml
    rsync --delete -avz _site/ ashriram@linux.cs.sfu.ca:/fas-info/cs/people/Faculty/ashriram/
