# Personal site

Built with Jekyll, Poole, Hyde theme, and Docker on Windows machine


`
docker run --rm --name=jekyll --label=jekyll --volume=c:/git/:/srv/jekyll -it -p 127.0.0.1:4000:4000 jekyll/jekyll:pages bash
`
`
docker start jekyll && docker attach jekyll
`

`
 jekyll s --incremental --force_polling
`

<img src='https://g.gravizo.com/svg?
 digraph G {
   main -> parse -> execute;
   main -> init;
   main -> cleanup;
   execute -> make_string;
   execute -> printf
   init -> make_string;
   main -> printf;
   execute -> compare;
 }
'/>
