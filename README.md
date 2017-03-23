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

![Alt text](https://g.gravizo.com/svg?
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)
