
chnage filemode from  100644 → 100755
git update-index --chmod=+x build.sh
and push changes again


LF will be replaced by CRLF the next time Git touches it(for wondows user)

This is actually difference because of line ending in linux/mac ((LF) character (represented as ‘\n’))
and Windows uses Carriage Return and Line Feed (CRLF) characters (‘\r\n’)
1.run command git config --list
2.and see if its having value core.autocrlf=true if its value is false then you can use   command:- git config core.autocrlf true 
3.if still you find issue execute command :- git config core.eol lf
4.if issue is still there then command :-git add --renormalize .   
5.if issue still not solved then delete cache git rm --cached  and if still not solved  re-install git
