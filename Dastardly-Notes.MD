#H1 Using Dastardly by [Portswigger](https://portswigger.net){:target="_blank"}

[DASTardly's Homepage]{https://portswigger.net/burp/dastardly "Dastardly's homepage")

Looking for a quick DAST (Dynamic application security testing) tool?  I've been focused on [DevSecOps](https://www.devsecops.org/) for a few years and passing along my testing.  


#Run Dastardly 
docker run --user $(id -u) --rm -v $(pwd):/tmp -e DASTARDLY_TARGET_URL=https://x.x.x.x: -e DASTARDLY_OUTPUT_FILE=/tmp/dastardly-report.xml public.ecr.aws/portswigger/dastardly:latest

Convert XML file to an HTML

sudo pip install junit2html 
git clone [https://github.com/inorton/junit2html](https://github.com/inorton/junit2html)

cd junit2html 
junit2html /tmp/dastardly-report.xml /tmp/dastardly-report.xml.html 
open /Applications/Safari.app /tmp/dastardly-report.xml.html 