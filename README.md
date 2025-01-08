Organize files into folders by last modified date, the folder name: last modified date, contains: files that share last modified date.

The tricky part here is how would you group the file by date:

1- My choice was a dictionary(string, list<string>)

2- "Foreach File in Folder" get the full path and last modified date

3- Check if: Dictionary.ContainsKey(LastModifiedDate) and then "Asign" new list: CurrentFile.FullName or add to the existing one.

4- Now, the move part, the folder names will be the dictionary key and the path will be the values.
