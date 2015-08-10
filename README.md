# unpack-jdk
How to install the JDK on windows without using the installer (to avoid potential bloat)

## Steps
* Download JDK
* Unpack the JDK installer with 7-zip (open it as a zip file)
* unpack the contents of tools.zip
* locate all the .pack-files (find . -iname "*.pack"
* run unpack200.exe for each pack-file with the pack-file as the first parameter and it's corresponding jar-file as the second parameter



example:  
bin/unpack200.exe jre/lib/charsets.pack jre/lib/charsets.jar  
bin/unpack200.exe jre/lib/deploy.pack jre/lib/deploy.jar  
bin/unpack200.exe jre/lib/ext/jfxrt.pack jre/lib/ext/jfxrt.jar  
bin/unpack200.exe jre/lib/ext/localedata.pack jre/lib/ext/localedata.jar  
bin/unpack200.exe jre/lib/javaws.pack jre/lib/javaws.jar  
bin/unpack200.exe jre/lib/jsse.pack jre/lib/jsse.jar  
bin/unpack200.exe jre/lib/plugin.pack jre/lib/plugin.jar  
bin/unpack200.exe jre/lib/rt.pack jre/lib/rt.jar  
bin/unpack200.exe lib/tools.pack lib/tools.jar  
