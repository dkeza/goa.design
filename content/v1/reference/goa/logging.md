+++
date="2019-05-09T20:22:44-07:00"
description="github.com/goadesign/goa/logging"
+++


# logging
`import "github.com/goadesign/goa/logging"`

* [Overview](#pkg-overview)
* [Index](#pkg-index)
* [Subdirectories](#pkg-subdirectories)

## <a name="pkg-overview">Overview</a>
Package logging contains logger adapters that make it possible for goa to log messages to various
logger backends. Each adapter exists in its own sub-package named after the corresponding logger
package.

Once instantiated adapters can be used by setting the goa service logger with WithLogger:

```go


	func main() {
	  // ...
	
	  // Setup logger adapter
	  logger := log15.New()
	
	  // Create service
	  service := goa.New("my service")
	  service.WithLogger(goalog15.New(logger))
	
	  // ...

}
```

See <a href="http://goa.design/implement/logging/">http://goa.design/implement/logging/</a> for details.




## <a name="pkg-index">Index</a>


#### <a name="pkg-files">Package files</a>
[doc.go](/src/github.com/goadesign/goa/logging/doc.go) 










- - -
Generated by [godoc2md](http://godoc.org/github.com/davecheney/godoc2md)
