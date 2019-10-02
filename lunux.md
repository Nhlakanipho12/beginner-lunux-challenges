 Task 1 : Basic Task

1.Type in ls and press enter. What do you see? What does this mean?
--I see a list of files and folders. The "ls" command lists all the files/folders in the current directory.

2.Type in pwd and press enter. What do you see? What does this mean? 
 --I see the names of folders. "pwd" command display the abosulute path,which is the name folders that you have accessed until you reach your working directory.

3.Make a new directory called workspace then cd into your new directory.
-- mkdir workspace

4.Type in ls and press enter. What do you see? What does this mean?
-- No files displayed. This means the directory/folder is empty.

5.Make a new file called README.md (you can use the touch command to do this)
-- Command: touch README.md

6.Make a copy of README.md, name your copy CHANGELOG.md.
-- Command:cp README.md CHANGELOG.md

Task 2 : Absolute and Relative Paths

Create an empty file named exercise.md and move this file to the /tmp directory, using a relative pathname. Then, delete this file using an absolute pathname.
-- Commands: touch exercise.md
-- mv exercise.mb workspace/tmp
-- rm tmp/exercise.md

Task 3 : cat commands
1.Create 3 files namely umuzi.md, recruits.md and cohort.md.
-- Commands: touch umuzi.md recruits.md cohort.md

2.Fill all 3 files with contents of your choice. Maybe some nice poems about you MUB experience.
-- Command: vim umuzi.md + enter button, press i button for insert mode, add content, press Esc button, Shift + colon, type "wq" to save and quit vim. Repeat the same steps to add the content to the rest of the files.

3.Write a script that concatenates the content of umuzi.md, recruit.md

-- Command: cat umuzi.md recruit.md cohort.md

4.Write a script that takes the content of umuzi.md, cohort.md and recruits.md to print/store the output into a new file named summary.md.

-- Command: cat umuzi.md recruit.md cohort.md > summary.md

5.Use the command line to append the words “The End” to summary.md. Be careful not to overwrite the exiting contend.
--Command: echo "The end." >> summary.md

Task 4 : The locate command
1.Write a script to help you locate a file named umuzi.
--Command: locate umuzi

2.Write a second script that will search for the same file and send the result of the search to a file named search_result.md.
--Command:locate umuzi > search_results.md

Task 5: The locate command cont..
1.Create a file within Documents directory, add to is a file named pad.md.
--Command:cd Documents, touch pad.md.

2.change the working directory to Desktop, then create a folder and name it work.
--Command: cd Desktop, mkdir work.

3.Copy pad.md to the currently working directory as pad_copy.md.
--Command:cp pad.md /home/recruit/Desktop/work/pad_copy.md.

4.Update the database used by locate by running locate updatedb.
--Command: locate updatedb

5.Change the working directory to the previous one (cd -).
--Command: cd Documents

6.Use locate to find pad_copy.md.
--Command: locate pad_copy.md

Task 6: Find commands
1.Write a script to find all files ending with ‘pdf’ on your computer.
--Command: find / -type f -name "*.pdf".

2.Write a second command that takes the result of the previous search and copy into a folder of your choice.
-- Command:find / -type f -name "*.pdf" > print_results.md

3.Write a command to display files that where modified today.
--Command: find . -mtime -1 -print

Task 7:Task 7 Text editor

1.Using nano text editor create a file named my_bio.md.

-- Command: nano my_bio.md 
2.Save the file and close the editor.
-- Ctrl + x
3.Create a folder named my_files and move my_bio.md within.
-- Command: mkdir my_files, mv my_bio.md my_files.
