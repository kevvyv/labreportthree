Kevin Yu
CSE 15
Lab 3


I have chosen to work with the grep command and observe its various outcomes and behaviors.

[Source for all commands](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

One interesting command line I have found with grep is the command `grep "^string" file_name`. This command searches within the given file and returns every instance of the string that is included after grep and this is extremely useful for parsing a large file for information you want.

the output is: ![image](https://user-images.githubusercontent.com/122575342/218666441-c6d55967-1a0e-4705-9144-793e57e47bb9.png)

However, when attempting to apply this to a directory, the result is:
	
![image](https://user-images.githubusercontent.com/122575342/218667001-c453ebad-3002-4a18-9f30-4f66cf695dc4.png)

Thus, suggesting that this command only works when searching within a file.

Another interesting command line I have found is the command `grep r "string" dir`. This command searches recursively within the directory and finds all instances of the string within all files inside the directory and this could prove extremely useful when wanting to do a deep search through a large directory.
	
The output for a directory name is:
![image](https://user-images.githubusercontent.com/122575342/218668316-19b021c6-c0bd-4fef-bc1a-ffa8eab81a80.png)

when searching within a file the result is:
![image](https://user-images.githubusercontent.com/122575342/218668579-8b8478e1-dca4-43c4-a334-c71194a0f841.png)
Which suggests that it now functions similarly to the normal grep command that searches within a file.
	
The third interesting command line I have found is the command `grep "string$" file_name` and this command searches within a file and returns all instances of a sentence ending with the given string. Although maybe not commonly used as the others, there could still be specific use cases for this.
	
The output for a file is:
![image](https://user-images.githubusercontent.com/122575342/218669855-5bf32cc5-5021-4543-b097-e0278609711d.png)

The output for a directory is:
![image](https://user-images.githubusercontent.com/122575342/218669956-8637670c-c7b1-4c0f-99c5-6f2fd416b52c.png)

Which demonstrates that this command does not work on directories.
	
The final interesting command line I have found is the command `grep "[character-character]" file_name`. This command searches the file for all instances where the specified range of characters show up and this could be useful when searching a large dataset and looking for specific characters.
	
The output for a file is:
![image](https://user-images.githubusercontent.com/122575342/218671309-ecb35bca-9067-47ec-92ce-1b38db9a5aeb.png)

The output for a directory is:
![image](https://user-images.githubusercontent.com/122575342/218671513-1edadf07-b19e-40e7-82de-76d0552bd9df.png)

This suggests that the command will not search through a directory for the specified characters.
