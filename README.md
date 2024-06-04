---
noteId: "25e4ef60226011efab86995c8100ea0e"
tags: []

---

# bash-aux



Collection of helpful functions for [bash](https://www.gnu.org/software/bash/).
Core functions are outlined below.

# Core functions

## Dependency checks

### check_dependencies
<pre class="r-output"><code>check_dependencies   
   Check whether multiple shell-commands are available

   Arguments:      
      --commands &lt;array&gt; 
         The commands to be checked for availability
         Default: ls chmod

   Usage:      
      check_dependencies \
         --commands "ls chmod"
</code></pre>

### check_dependency
<pre class="r-output"><code>check_dependency   
   Check whether a single shell-commands is available

   Arguments:      
      --command  &lt;str&gt; 
         The command to be checked for availability
         Default: ls

   Usage:      
      check_dependency \
         --command  "ls"
</code></pre>

## Folders & Files

### current_file
<pre class="r-output"><code>current_file   
   Determine the current file path, using 
   bash    : ${BASH_SOURCE[0]}                                         
   zsh     : ${(%):-%x}                                              

   Usage:      
      current_file
</code></pre>

### make_file_path
<pre class="r-output"><code>make_file_path   
   Create file from path, create path if it does not exist

   Arguments:      
      --file     &lt;str&gt; 
         The file to create the path for
         Default: ~/path/to/file

   Usage:      
      make_file_path \
         --file     "~/path/to/file"
</code></pre>

### normalize_path
<pre class="r-output"><code>normalize_path   
   Normalize a folder / file path

   Arguments:      
      --path     &lt;str&gt; 
         The path to normalize
         Default: ~/path/to/file

   Usage:      
      normalize_path \
         --path     "~/path/to/file"
</code></pre>

### read_from_file
<pre class="r-output"><code>read_from_file   
   Read a file.
   Like `cat`, but returns empty string if file does not exist

   Arguments:      
      --file     &lt;str&gt; 
         The file to read from
         Default: ~/path/to/file

   Usage:      
      read_from_file \
         --file     "~/path/to/file"
</code></pre>

## Logging

<pre class="r-output"><code>bash_aux_log   
   Create log files based on the called function's name

   Arguments:      
      --path     &lt;str&gt; 
         The path to create the log files in
         Default: /Users/simonlenau/Projects_Personal/bash-aux

   Usage:      
      bash_aux_log \
         --path     "/Users/simonlenau/Projects_Personal/bash-aux"
</code></pre>

## Misc

### read_non_blocking
<pre class="r-output"><code>read_non_blocking   
   Read input from stdin / pipe / user input, but don't wait for the input

   Usage:      
      read_non_blocking
</code></pre>
