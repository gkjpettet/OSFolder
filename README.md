# OSFolder

A replacement for the built-in `SpecialFolder` methods that returns a `Xojo.IO.FolderItem` rather than a classic `FolderItem`. It just helps to make code a little easier to read.

For example, with Xojo's built-in methods, in order to get a reference to the Desktop as a `Xojo.IO.FolderItem` (rather than the classic `FolderItem`) you'd need to do this:

```
dim desktop as Xojo.IO.FolderItem = New Xojo.IO.FolderItem(SpecialFolder.Desktop.NativePath.ToText)

```

Now you can just do this:

```
dim desktop as Xojo.IO.FolderItem = OSFolder.Desktop
```

Much nicer.
