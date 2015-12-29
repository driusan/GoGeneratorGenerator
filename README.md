# Go Generator Generator

Go Generator Generator is a tool to generate Go
programs which generate Go code with "go generate".

## What?

This is a tool to write the boilerplate needed to write
programs in Go which function as code generation tools
that can be invoked with "go generate".

## What?

Executing `GoGeneratorGenerator x` will create a directory
`x` with boilerplate code in it for a program that, when 
invoked with `go generate`, will write a file which contains
the appropriate package name, a DO NOT EDIT comment, and 
the automatically generated code. The default generated
code is a comment saying "YOUR GENERATED CODE GOES HERE."

It's expected that you'll use the generated code as a starting
point to write a program which does something more interesting,
like working around the fact that Go doesn't have generics.

If this still doesn't make sense, read about 
[go generate](https://blog.golang.org/generate). 

(Instead of running this tool, you can copy the SampleStub 
directory, which contains the output of
`GoGeneratorGenerator SampleStub` as a starting point for your
code generation program, but that wouldn't be as meta.)
