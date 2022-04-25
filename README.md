# Index Local Folders to XML File with RunSpace

This is a Proof of concept - Alpha

I am hopping to get some input on how I could improve my coding

Have a nice day 🤠

Wøødy

	.SYNOPSIS
		This Script generates a index file using RunSpace 
	.DESCRIPTION
		It first build a tree of the folder you select.
		From that tree, it adds the files contained in the tree.
	.NOTES
		It does not follow Symbolic Links.
		It is not designed for use on networks drives or UNC Paths
	.FUNCTIONALITY
		Recommended install:
			Create a folder and place the script inside that folder
	.EXAMPLE 
		To view content of the file you can use:
		Simply navigate to the Data folder and 
		(Import-Clixml Name-Of-The-File.xml) | Out-GridView
		You can sort and filter within the Out-GridView
		or
		$Variable = Import-Clixml .\D-Download-Keep-for-a-Bit.xml
		$Variable | Out-GridView
	.OUTPUTS
		The (xml) files contain the following information
		From the files and folders it gathers:
		FullName, Name, Attributes, Directory, Extension, Length, 
		CreationTimeUtc, LastAccessTimeUtc,	LastWriteTimeUtc
			
		For the prurpose of Indexing and Reporting, the Script Generates:
		Files #, Folders #, Junction's , Depth#
	.OUTPUTS
		The following folders are created where you run the script from.
		Data - This is where the Index files are saved
		Log-Files - Transcript are enabled by default. 
		
	.NOTES
		Special shout out to Powershell Discord Community.
		There help has been invaluable and I am forever Greatfull
		Drop in and say hi if you have a chance and say hello
		
		https://discord.com/invite/powershell
	
