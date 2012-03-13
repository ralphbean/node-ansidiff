ansidiff -- a small node.js library for ANSI colored text diffs


# Usage

    var ansidiff = require('ansidiff');
    var log = console.log;
    log( ansidiff.chars('will work for food', 'will code for foo') );
    log( ansidiff.words('will work for food', 'will code for foo') );
    log( ansidiff.lines('one\ntwo\nthree', 'one\ndeux\ntrois\nthree') );
    log( ansidiff.css('#body { color: blue }', '.content { color: blue }') );

These are using the default `bright` colorer. You can use the `subtle`
one if you wish:

    log( ansidiff.words('will work for food', 'will code for foo', ansidiff.subtle) );

![ansi color diffs]()


# Install

    npm install ansidiff


# License

MIT.


var ansidiff = require('ansidiff');
var log = console.log;
log( ansidiff.chars('will work for food', 'will code for foo') );
log( ansidiff.words('will work for food', 'will code for foo') );
log( ansidiff.lines('one\ntwo\nthree', 'one\ndeux\ntrois\nthree') );
log( ansidiff.css('#body { color: blue }', '.content { color: blue }') );