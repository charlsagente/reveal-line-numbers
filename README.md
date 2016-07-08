# Plain Text Block Line Numbers

## Overview

A simple 'library' for adding line numbers and hightlighting specific lines of plain text like log files.


## Usage

### Adding line numbers to code blocks
To add line numbers to a code block, just add the class 'line-numbers' to the &lt;code> element

```html
<pre><code class="line-numbers">
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
log4j:WARN No appenders could be found for logger (org.elasticsearch.plugins).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
</code></pre>
```

### Highlighting line numbers.

To highlight particular line numbers in a text block, add the attribute 'data-highlight-lines' to the &lt;code> element.
* Seperate the lines you would like to highlight with a comma(,).
* Specifcy a group of lines to highlight by seperating the start line and end line with a dash(-).

![line_codes](https://cloud.githubusercontent.com/assets/948024/16702973/57222488-452f-11e6-8f30-124e8c3d61de.jpg)

_Example: to highlight the lines 1,2,3:_

```html
<pre><code class="line-numbers" data-highlight-lines="1,2,3">
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
log4j:WARN No appenders could be found for logger (org.elasticsearch.plugins).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
</code></pre>
```

_Example: To highlight the lines 4 to 10:_

```html
<pre><code class="line-numbers" data-highlight-lines="4-10">
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
log4j:WARN No appenders could be found for logger (org.elasticsearch.plugins).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
</code></pre>
```

_Example: highlighting lines 1 to 3 and 5,7,9:_

```html
<pre><code class="line-numbers" data-highlight-lines="1-3,5,7,9">
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
log4j:WARN No appenders could be found for logger (org.elasticsearch.plugins).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
</code></pre>
```
