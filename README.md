# ckfinder_java_2.6.2.1
在原来的基础上，修改了FileUploadCommand 类中的 getFinalFileName 方法。
原来是上传重名后，显示上传失败，实际上传成功，显示空的图片，不能删除，那是因为重名为（1）的样式，这样的文件是有问题的，名称不能有（）。修改后直接加1，而没有（）
