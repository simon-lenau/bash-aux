bash-aux
================

Auxiliary functions to be used in bash

# Core functions

## Dependency checks

### check_dependencies

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
check_dependencies   
   Check whether multiple shell-commands are available
&#10;   Arguments:      
      --commands &lt;str&gt; 
         The commands to be checked for availability
         Default: ls chmod
&#10;   Usage:      
      check_dependencies \
         --commands "ls chmod"
</code></pre>

### check_dependency

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
check_dependency   
   Check whether a single shell-commands is available
&#10;   Arguments:      
      --command  &lt;str&gt; 
         The command to be checked for availability
         Default: ls
&#10;   Usage:      
      check_dependency \
         --command  "ls"
</code></pre>

## Folders & Files

### current_file

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
current_file   
   Determine the current file path, using 
   bash    : ${BASH_SOURCE[0]}                                         
   zsh     : ${(%):-%x}                                              
&#10;   Usage:      
      current_file
</code></pre>

### make_file_path

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
make_file_path   
   Create file from path, create path if it does not exist
&#10;   Arguments:      
      --file     &lt;str&gt; 
         The file to create the path for
         Default: ~/path/to/file
&#10;   Usage:      
      make_file_path \
         --file     "~/path/to/file"
</code></pre>

### normalize_path

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
normalize_path   
   Normalize a folder / file path
&#10;   Arguments:      
      --path     &lt;str&gt; 
         The path to normalize
         Default: ~/path/to/file
&#10;   Usage:      
      normalize_path \
         --path     "~/path/to/file"
</code></pre>

### read_from_file

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
read_from_file   
   Read a file.
   Like `cat`, but returns empty string if file does not exist
&#10;   Arguments:      
      --file     &lt;str&gt; 
         The file to read from
         Default: ~/path/to/file
&#10;   Usage:      
      read_from_file \
         --file     "~/path/to/file"
</code></pre>

## Misc

### read_non_blocking

<pre class="r-output"><code>BASH_AUX_DIR: /Users/simonlenau/Projects_Personal/bash-aux
BASH_DOC_DIR: /Users/simonlenau/Projects_Personal/bash-aux/submodules/bash-doc
read_non_blocking   
   Read input from stdin / pipe / user input, but don't wait for the input
&#10;   Usage:      
      read_non_blocking
</code></pre>
