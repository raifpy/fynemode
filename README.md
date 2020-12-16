# How it's working

Compile go codes (c-shared):

    go build -ldflags="-w -s" -buildmode="c-shared" -o /tmp/xxxxxxx/libxxx.so
  
add run perm library(chmod +x):

    chmod +x /tmp/xxxxxx/libxxx.so
        
        
upx \<libName\>.so

    upx --android-hslib /tmp/xxxxxxx/libxxx.so
      

# You need install upx

    apt install upx
    dnf install upx
      
i don't know upx is avaible on Windows.

Since fyne codes have been changed afterwards, you probably won't be able to compile the current codes even if you pull them via "go get" - even if it is, it might not work properly.

So I upload files compiled for Windows and Linux.
You can use it directly by throwing it to the PATH position. | Releases |

Also i append Android INTERNET permission default AndroidManifest.xml

Enjoy..

<img src="https://github.com/raifpy/fynemode/blob/main/resource/fyneMode.png">
<img src="https://github.com/raifpy/fynemode/blob/main/resource/r.png">
<img src="https://github.com/raifpy/fynemode/blob/main/resource/r2.png">
