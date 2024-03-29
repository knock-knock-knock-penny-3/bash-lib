# Bash lib

This project provides a simple bash library for use within devops scripts, deployment scripts or CLIs


## How to use the library

To use the only library currently available, simply include it within your script via `source`

> source */path/to/library/* stdout<br>
> . */path/to/library/* stdout

At this point you can use the public methods present in the library:

- ### log

<u>Usage:</u><br>
`log "message"`<br>
<br>
If the `CLI_DEBUG` environment variable is set to 1 this method prints a line formatted like this:<br>
== *script_name* *timestamp* *message*

- ### warning

<u>Usage:</u><br>
`warning "message"`<br>
`warning "message %s" "replacement"`<br>
<br>
This method prints `message` in yellow<br>
If `message` contains a conversion specification this is replaced with `replacement`, if present, which will be printed in bold

- ### error

<u>Usage:</u><br>
`warning "message"`<br>
`warning "message %s" "replacement"`<br>
<br>
This method prints `message` in red<br>
If `message` contains a conversion specification this is replaced with `replacement`, if present, which will be printed in bold


- ### success

<u>Usage:</u><br>
`warning "message"`<br>
`warning "message %s" "replacement"`<br>
<br>
This method prints `message` in green<br>
If `message` contains a conversion specification this is replaced with `replacement`, if present, which will be printed in bold


- ### msg

<u>Usage:</u><br>
`warning "message"`<br>
`warning "message %s" "replacement"`<br>
<br>
This method prints `message` in blue<br>
If `message` contains a conversion specification this is replaced with `replacement`, if present, which will be printed in bold

