---
title: Open File Dialog
page_title: Open File Dialog
description: Open File Dialog
slug: radcloudupload-features-custom-open-file-dialog
tags: open,file,dialog
published: True
position: 4
---

# Open File Dialog





## 

The __RadCloudUpload__ exposes the __CreateOpenFileDialog__ property. It is of type __Func<[OpenFileDialog](http://msdn.microsoft.com/en-us/library/microsoft.win32.openfiledialog%28v=vs.110%29.aspx)>__ and can be used to get or set a custom open file dialog. You can use this property to restrict users to upload certain type of files.
        

#### __XAML__
    xCloud.CreateOpenFileDialog = () =>
    {
        OpenFileDialog ofd = new OpenFileDialog();
        ofd.Filter = "txt files (*.txt)|*.txt|All files (*.*)|*.*";
        return ofd;
    };



# See Also

 * [Providers]({%slug radcloudupload-features-providers%})
