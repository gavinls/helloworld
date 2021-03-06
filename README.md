## Managing Complex Server Systems Using Docker

This project is a demo showing how to use Docker to manage a system
consisting of more than one programs.

It contains two programs -- a search engine server (`searchengine`)
and an indexer daemon (`indexer`).  `searchengine` is an HTTP server,
which accepts queries and returns search results by looking up a data
structure known as *index*.  It is also an RPC server, which accepts
index updates generated by `indexer`, which sends new indexes to
`searchengine` once a second.

Using this project as an example, I wrote a blog post,
[Docker: A Revolution of Development, Test and Deployment](http://cxwangyi.github.io/story/docker_revolution_1.md.html),
to show you how to manage systems of micro-service architecture using
Docker.
