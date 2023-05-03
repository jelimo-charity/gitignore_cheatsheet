Pattern|Explanation/Matches |Examples
-----        |  ------------  | --------     
name.file | All names with name.file will be ignored    | /name.file <br>  /lib/name.file 
name.html | All files with name.html will be ignored    | /name.html

<ul><li>A blank line matches no files, so it can serve as a separator for readability.</li>

<li>A line starting with # serves as a comment. Put a backslash ("\") in front of the first hash for patterns that begin with a hash.</li>

<li>Trailing spaces are ignored unless they are quoted with backslash ("\").</li>

<li>The slash / is used as the directory separator. Separators may occur at the beginning, middle or end of the .gitignore search pattern.</li>

<li>If there is a separator at the beginning or middle (or both) of the pattern, then the pattern is relative to the directory level of the particular .gitignore file itself. Otherwise the pattern may also match at any level below the .gitignore level.</li>

<li>If there is a separator at the end of the pattern then the pattern will only match directories, otherwise the pattern can match both files and directories.

<li>For example, a pattern doc/frotz/ matches doc/frotz directory, but not a/doc/frotz directory; however frotz/ matches frotz and a/frotz that is a directory (all paths are relative from the .gitignore file).</ul>
                                                                                                  

