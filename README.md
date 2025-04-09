# smithy4s-example

## build

The mill smithy4s plugin uses the smithy file in `example/smithy/ExampleService.smithy` to generate classes in `out/example/smithy4sOutputDir.dest/scala/smithy4s/example/hello`.

The service implementation in `example/src/Main.scala` uses those generated classes.

## run

```
mill example.run
```

Open http://localhost:9000/docs in a browser to use the generated OpenAPI UI.

Or
```
curl -X 'POST' \
  'http://localhost:9000/Neil?town=Ottawa' \
  -H 'accept: application/json' \
  -d ''
```

## references
Great docs at https://disneystreaming.github.io/smithy4s/docs/overview/intro/