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

![Alt text](https://g.gravizo.com/source/custom_mark2?https%3A%2F%2Fraw.githubusercontent.com%2FTLmaK0%2Fgravizo%2Fmaster%2FREADME.md)
<!---
custom_mark2
@startuml
object Object01
object Object02
object Object03
object Object04
object Object05
object Object06
object Object07
object Object08

Object01 <|-- Object02
Object03 *-- Object04
Object05 o-- "4" Object06
Object07 .. Object08 : some labels2
@enduml
custom_mark2
-->
