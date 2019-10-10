 rosetta
==========

### General Programming Challenges

- Write a program which prints "hello world"
- Write a simple `echo` program, which prints it's command-line arguments
```
$ ./echo hello world
hello world
```
- Write a simple implementation of `cat` command
- Write a simple implementation of `uniq` command.

> uniq [input_file [output_file]]
> The uniq utility reads the specified input_file comparing adjacent lines, and writes a copy of each unique input line to the output_file.  If input_file is a single dash ('-') or absent, the standard input is read.  If output_file is absent, standard output is used for output. 

- Write a simple implementation of `curl` command (Just fetching of URLs). Try writing a sequential version & concurrent version.

```
$ ./curl https://google.com https://stackoverflow.com
```
- Write a program which recursively finds all the links in a HTML document & prints in the stdout.

- Implement a concurrent ftp server. The server should interpret commands from each client such as `cd` to change directory, `ls` to list a directory, `get` to send the contents of file, and `close` to close the connection. You can use the standard `ftp` command as client, or write your own.

- Write a program `crawler` which accepts a website as input and makes local copies of the pages it finds, creating directories as necessary. Don’t make copies of pages that come from a different domain. For example, if the original page comes from golang.org, save all files from there, but exclude ones from vimeo.com. Make this concurrent as possible. 

- Write a simple implementation of `wc`

> wc [file ...]
> The wc utility displays the number of lines and words in each input file, or standard input (if no file is specified) to the standard output. 

- Write a simple implementation of `du` command

- The popular web comic xkcd has a JSON interface. For example, a request to https://xkcd.com/571/info.0.json produces a detailed description of comic 571, one of many favorites. Download each URL (once!) and build an offline index. Write a tool xkcd that, using this index, prints the URL and transcript of each comic that matches a search term provided on the command line.

- The JSON-based web service of the Open Movie Database lets you search https://omdbapi.com/ for a movie by name and download its poster image. Write a tool poster that downloads the poster image for the movie named on the command line.

- Implement a clock server. Clients opens a tcp connection on particular port. Server sends client current time every second, until client closes connection. Expand on the same to handle multiple clients concurrently.

- Write a simple implementation of `netcat` command.

- Write a concurrent echo server, which echos the message that client sent.
- Write a expressions evaluator. Our expression language consists of floating-point literals; the binary operators `+, -, *,` and `/;` the unary operators `-x` and `+x`; function calls `pow(x,y)`, `sin(x)`, and `sqrt(x)`; variables such as `x` and `pi`; and of course parentheses and standard operator precedence. All values are of type float64. Here are some example expressions:

```
sqrt(A / pi)
pow(x, 3) + pow(y, 3)
(F - 32) * 5 / 9
```

- Write sqlite db from scratch.

- Write a simple implementation of `slack` app. User can send messages to other users. Users are part of a channel. All messages in channel are broadcasted to all users in that channel. Users can join & leave channel. 

- Write a simple `twitter` web app. User can add new tweet, read all tweets, update an existing tweet & delete a tweet. You'll have to develop appropriate REST APIs. Expand the app to maintain tweets for different persons. Add more actions like "retweet", "like". Handle notifications to users. Scale this model for large number of users.
