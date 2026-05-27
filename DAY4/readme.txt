DEEp dive into git Commit

branch is created only when the first commit is done
[D[D[A1.[B[D[D
2.SHA1  (Secure Hashing Algorithm 1) is used for encryption
   ->it is a 40 character alphanumberic number
3.git command are stored in .git/ folder,in that ,in objects folder all commit are stored [D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D
		->dont make any chnages to it
4.if i have done i have commit and it has 2 files.lets say first commit as c1
  ->now i do 2nd commit which have 2 files and [A[A[B[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C and currently head is pointing to c1[B[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D now its c2 and it has 4 files now it takes reference of c1 commit 

5.Now i have commited and now i have modified the file which i commited 
  ->but now git aware of old content not the new content
  ->if i do git status it gives modified with file name

[D[A  ->now i have to bring to staging area with git command git add file name

[A[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C and i have to commit 
  ->but it will create a new commit .Now i dont want this to happen because for that file already one commit is done 
  ->so for that i will modify that commit only using
[D[D[D[D[D-> git commit -a -m "modified f4.txt"

6.[A[A[A[A[A[A[B[B[B[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[A[A[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[B[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C
[A[B[C[C[C[C
[A[A[B[B[C[A[C[C[Ceach time if all files are modified and i have to do git add . and then i do commit is not good.just do below commit for the same file whic prebiously commited will get this new commit[C[C[C[C[C[C[C[C[C[C[C ->new commit message 
  ->git commit -a -m"modified f4.txt"
[C
6.Already done a commit but  how do i mmodify that commit

[C[C[Cf4.txt ka commit hai and now i add temp.txt .
  ->[A[A[D[B->f->f4.txt ka commit hai aur abhi temp.txt file add karunga[B[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[Dabhi temp.txt ka commit na bana karke f4.txt ke commit mein eske add karnege

[A  ->git commit -amend 

7.i want to amend but dont want to modify the commit message
  -->git commit -[A[A[D[A-[C[B[B[B[D-amend--no-edit

8.how to sign off a commit or how to give a signature  (used when my project is over i.e after testing and reviewing)
  ->git commit -s -m"task done"[D[D[D[D[D[D[D[D[D[D[D [D"[D[C[C[C[C[C[C[C[C[C[C[C[C[C[C

9.how do i create empty commits 
   ->used when i want to trigger ci pipleines without adding multiple files and commit instaed of creating files and adding 
   ->just to empty commit (from that easily ci pipelines are trigerred without creating multiple files
   ->git commit -alloq-empty- -m"Dummy"[D[C[D[D[D[D[D[D[D[Dy[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[D[w[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C[C
