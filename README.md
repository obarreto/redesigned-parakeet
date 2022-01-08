# redesigned-parakeet

<pre><font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>/home</b></font>$ ls
<font color="#3465A4"><b>ozeias</b></font>
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>/home</b></font>$ cd ozeias/
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~</b></font>$ mkdir workspace
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~</b></font>$ cd workspace/
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace</b></font>$ git clone git@github.com:obarreto/redesigned-parakeet.git
Cloning into &apos;redesigned-parakeet&apos;...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace</b></font>$ cd redesigned-parakeet/
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch
* <font color="#4E9A06">main</font>
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ echo arquivo1.txt
arquivo1.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ status

Command &apos;status&apos; not found, did you mean:

  command &apos;statup&apos; from snap statup (0.79.91)
  command &apos;statfs&apos; from deb gocryptfs (1.7.1-1)
  command &apos;states&apos; from deb enscript (1.6.5.90-3)
  command &apos;qstatus&apos; from deb gridengine-client (8.1.9+dfsg-9build2)

See &apos;snap info &lt;snapname&gt;&apos; for additional versions.

<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch main
Your branch is up to date with &apos;origin/main&apos;.

nothing to commit, working tree clean
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ ls
README.md
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ echo &gt; arquivo1.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch main
Your branch is up to date with &apos;origin/main&apos;.

Untracked files:
  (use &quot;git add &lt;file&gt;...&quot; to include in what will be committed)
	<font color="#CC0000">arquivo1.txt</font>

nothing added to commit but untracked files present (use &quot;git add&quot; to track)
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git add *
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch main
Your branch is up to date with &apos;origin/main&apos;.

Changes to be committed:
  (use &quot;git restore --staged &lt;file&gt;...&quot; to unstage)
	<font color="#4E9A06">new file:   arquivo1.txt</font>

<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git commit -m &quot;adiciona artquivo na branch main&quot;
[main 4e640e7] adiciona artquivo na branch main
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo1.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 6 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 289 bytes | 289.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:obarreto/redesigned-parakeet.git
   06ff0bf..4e640e7  main -&gt; main
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git checkout -b &apos;nova-funcionalidade&apos;
Switched to a new branch &apos;nova-funcionalidade&apos;
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch 
  main
* <font color="#4E9A06">nova-funcionalidade</font>
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ echo &gt; arquivo2.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch nova-funcionalidade
Untracked files:
  (use &quot;git add &lt;file&gt;...&quot; to include in what will be committed)
	<font color="#CC0000">arquivo2.txt</font>

nothing added to commit but untracked files present (use &quot;git add&quot; to track)
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git checkout main
Switched to branch &apos;main&apos;
Your branch is up to date with &apos;origin/main&apos;.
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch
* <font color="#4E9A06">main</font>
  nova-funcionalidade
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch main
Your branch is up to date with &apos;origin/main&apos;.

Untracked files:
  (use &quot;git add &lt;file&gt;...&quot; to include in what will be committed)
	<font color="#CC0000">arquivo2.txt</font>

nothing added to commit but untracked files present (use &quot;git add&quot; to track)
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git checkout nova-funcionalidade 
Switched to branch &apos;nova-funcionalidade&apos;
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch
  main
* <font color="#4E9A06">nova-funcionalidade</font>
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch nova-funcionalidade
Untracked files:
  (use &quot;git add &lt;file&gt;...&quot; to include in what will be committed)
	<font color="#CC0000">arquivo2.txt</font>

nothing added to commit but untracked files present (use &quot;git add&quot; to track)
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git add *
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch nova-funcionalidade
Changes to be committed:
  (use &quot;git restore --staged &lt;file&gt;...&quot; to unstage)
	<font color="#4E9A06">new file:   arquivo2.txt</font>

<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git commit -m &quot;Adiciona arquivo 2 na branch nova&quot;
[nova-funcionalidade 5adffdc] Adiciona arquivo 2 na branch nova
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo2.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch 
  main
* <font color="#4E9A06">nova-funcionalidade</font>
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git push origin nova-funcionalidade
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 6 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 287 bytes | 287.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for &apos;nova-funcionalidade&apos; on GitHub by visiting:
remote:      https://github.com/obarreto/redesigned-parakeet/pull/new/nova-funcionalidade
remote: 
To github.com:obarreto/redesigned-parakeet.git
 * [new branch]      nova-funcionalidade -&gt; nova-funcionalidade
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git checkout main 
Switched to branch &apos;main&apos;
Your branch is up to date with &apos;origin/main&apos;.
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git branch
* <font color="#4E9A06">main</font>
  nova-funcionalidade
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git merge nova-funcionalidade 
Updating 4e640e7..5adffdc
Fast-forward
 arquivo2.txt | 1 <font color="#4E9A06">+</font>
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo2.txt
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git status
On branch main
Your branch is ahead of &apos;origin/main&apos; by 1 commit.
  (use &quot;git push&quot; to publish your local commits)

nothing to commit, working tree clean
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ git push origin main 
Total 0 (delta 0), reused 0 (delta 0)
To github.com:obarreto/redesigned-parakeet.git
   4e640e7..5adffdc  main -&gt; main
<font color="#4E9A06"><b>ozeias@barreto</b></font>:<font color="#3465A4"><b>~/workspace/redesigned-parakeet</b></font>$ 
</pre>
