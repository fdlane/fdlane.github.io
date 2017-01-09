# Personal site

Built with Jekyll, Poole, Hyde theme, and Docker on Windows machine


`
docker run --rm --name=jekyll --label=jekyll --volume=c:/git/:/srv/jekyll -it -p 127.0.0.1:4000:4000 jekyll/jekyll:pages bash
`
docker start jekyll  && docker attach jekyll

`
 jekyll s --incremental --force_polling
`