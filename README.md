# hl

Output Highlighter

Uses grep to merely highlight the search string from the input stream rather  
than isolate it.  Great for use with scontrol show job                        
                                                                                
https://superuser.com/questions/914856/display-all-output-but-highlight-search-matches/914862
                                                                                
Usage : hl root /etc/passwd                                                   
      : command | hl string                                                   
                                                                                
grep -i --color=always -e "^" -e "$@" 
