# G729-PJSIP-2.6-VISUALC-WINDOWS
G729 integrated into PJSIP 2.6 for Visual Studio C on Windows


G.729 implementation included in this project is Open Source based on Belledonne Communications implementation. If you want to use it in your app, you have to get a license from G.729 patent holders for every device on which you're going to use it. The authors of this project and of the open source implementation are not responsible for improper or unlicensed use of G.729 codec.

This patch allows you to include G.729 in your pjsip 2.6 on windows, using Visual Studio 2008 or latest.

# HOW TO INTEGRATE G729 in your current VisualStudio pjproject 2.6:

1. Unzip pjproject-2.6_G729-YYYYMMDD.zip (Currently is 20180410)

2. Copy audio_codecs.c into your pjproject-2.6\pjmedia\src

3. Copy config.h into your pjproject-2.6\pjmedia\include

4. Copy g729.h into your pjproject-2.6\pjmedia\include

5. Copy g729.c into your pjproject-2.6\pjmedia\src

6. Copy pjmedia-codec.h into your pjproject-2.6\pjmedia

7. Copy directory bcg729 into your pjproject-2.6\pjmedia\src\pjmedia-codec

8. Add g729.h, g729.c and directory bcg729 into your project pjmedia_codec

9. Modify your config_site.h located at pjproject-2.6\pjlib\include\pj\ and add:

#define PJMEDIA_HAS_G729_CODEC    1


10. Rebuild your pjmedia_codec and samples project

11. Enjoy!



# =============================================
# Feel free to contact me at madinix@gmail.com
